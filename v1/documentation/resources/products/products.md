# Products 

## Products description
Products is a collection of all available travel products in the categories:   
- Day Trips  
- Accomodation  
- Packages  
- Transfers  
- Other services

Resource     | Description | Mandatory Parameters| Optional Parameters|
----------- | ----------- | ||
 GET http://api.aventuradobrasil.com/v1/products | RETURNS all products featuring, id, category, region, description, pax, unit price, extra Information if available | 
GET http://api.aventuradobrasil.com/v1/products/search | RETURNS a specific range of products which is matching the filtering parameters. | from_date, to_date, region, category, pax. | name |   
 


## Example: Query all products

"products" => [  
{
      
"id": "34",
      
"name": "Hotel Bellevue",
      
"description": "A great place for wildlife watching,
    
"extrainfo": "DBL Suite deluxe",
  
"price": "250",
  
"region": "Minas",
  
"category": "Accomodation",
  
"pax": "3"

} 

{


"id": "4",

"name": "Guide for Manaus Rio Adventure",

"description": "24h walking Guide for Manaus Rio Adventure",

"extrainfo": "A great place for wildlife watching",

"price": "25",

"region": "amazonia",

"category": "Day Trips",

"pax": "5"
 
 }]

## Example: Query particular product
 
 {
  
"request_summary" =>  
{
        
"from_date": "2014-04-03",
        
"to_date": "2014-04-07",
        
"region": "Rio",
        
"category": "Accomodation",
  
"pax": "2"
      
},
   
"products" => [
      
{
        
"id": "34",
        
"name": "Hotel Copacabana",
        
"description": "Luxurious Hotel ...",
        
"extrainfo": "Honeymoon Suite",
        
"price": "750",
          
"amount": "1,000"
      
},
      
{
        
"id": "55",
        
"name": "Hotel california in Rio"
        
"description": "Romantic getaway",
        
"extrainfo": "Kingsize room",
        
"price": "100",
        
"amount": "400"
    }
  ]
}
 
