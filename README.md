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

Getting param from url is also possible:  
![alt text](https://github.com/saprykins/logic_app_handover-variables-via-body/share variable via url_v2.png?raw=true)


adding storage  
create storage account  
create blob -> container -> private, ex: "Log" is name of container  

in logic app:  
between request and response add action  
action -> blob -> create blob (file) // it will create new file  
establish connection with blob  
Connection name:= new; much more details here https://learn.microsoft.com/en-us/azure/connectors/connectors-create-api-azureblobstorage?tabs=consumption  
result: 
you put variable in url, the variable in file, file name

steps and params handover here  
https://www.youtube.com/watch?v=M_qdupbfThA  

logic here  
https://www.youtube.com/playlist?list=PLJK9-fn-j_0WaWL0w2bTycipgoxxaK_Mm  
