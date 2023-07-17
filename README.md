# logic_app_handover-variables-via-body

source link: https://www.youtube.com/watch?v=JWeirfucJOA  

Goal: we have someone who clicks on web-page, it shows us "hello world"  
1/ request  
get  
2/ response  
get  
// no variables  


Goal: we have someone who sends request from postman with variables in request body, in postman we see reply with the use of variables  
1/ request:   
a) post  
b) specify request body json schema  
{  
  "state": "value1",  
  "date":"value2"  
}  
2/ response  
in postman  
a) POST  
b) Header: Content-Type:= application/json  
c) Body:   
{  
  "state": "ok",  
  "date":"20/03/23"  
}  
