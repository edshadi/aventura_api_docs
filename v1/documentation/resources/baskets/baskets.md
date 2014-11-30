## Baskets (journey packages) description
Baskets is a collection of all the journey packages featuring product selections you have booked for your clients



Resource     | Description | MANDATORY PARAMETERS | Return|
:----------- | :-----------: | :-----------: | :-----------: |
GET http://api.aventuradobrasil.com/v1/baskets| RETURNS all your baskets featuring all product information| | |
GET http://api.aventuradobrasil.com/v1/basket/id | RETURNS your particularly requested basket featuring all its product information        | | |
 POST http://api.aventuradobrasil.com/v1/baskets | CREATE or ADD a basket with a selection of products featuring the following mandatory information: | journey name (basket name), product id, from date, to date, pax | Status 200  | 
PUT http://api.aventuradobrasil.com/v1/baskets | MODIFY or DELETE a basket with a selection of products featuring the following mandatory information | journey name, product id, action=remove OR update,  From date, To date, pax | Status 200 | 
DELETE http://api.aventuradobrasil.com/v1/baskets | MODIFY or DELETE a basket with a selection of products featuring the following mandatory information: | journey_name | Status 200 | 

## Example: Query all your baskets 

{
    
"baskets" =>
      
{
        
"Trip to Rio including city guide" =>
          
[
            
{
              
"product_id": "155",
              
"from_date": "2014-04-03",
              
"to_date": "2014-04-08",
              
"accomodation": "1",
              
"package": "0",
              
"nights": "5",
              
"Pax" : "2"
            
},
            
{
              
"product_id": "83",
              
"from_date": "2014-04-04",
              
"to_date": "2014-04-06",
              
"accomodation": "0",
              
"package": "1",
              
"nights": "2",
              
"Pax" : "2"
            
}
          
],
          
"Florianopolis Family trip" =>
            
[
             
 {
               
 "product_id": "13",
                
"from_date": "2014-04-04",
               
 "to_date": "2014-04-14",
                
"accomodation": "1",
                
"package": "1",
                
"nights": "2",
               
 "Pax" : "2"
              
},
              
{
                
"product_id": "185",
                
"from_date": "2014-04-05",
               
 "to_date": "2014-04-06",
                
"accomodation": "0",
                
"package": "0",
                
"nights": "0",
                
"Pax" : "2"
              
}
          ]
      }
}
## Example: Query a particular basket

{  
"Florianopolis Family trip" =>  
[
  
{
  
"product_id": "13",  
                
"from_date": "2014-04-04",
                
"to_date": "2014-04-14",
                  
"accomodation": "1",
                
"package": "1",
                
"nights": "2",
                
"Pax" : "2"
              
},
              
{
                
"product_id": "185",
                
"from_date": "2014-04-05",
                
"to_date": "2014-04-06",
                
"accomodation": "0",
                
"package": "0",
                
"nights": "0",
                
"Pax" : "2"
              
}]}
 

 
