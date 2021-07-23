
## Rest APIs:

* DynamoDB - storage
* Go - Language for MS
* 2 EC2 instance - to deploy our microservice
* ALB - Application Load Balancer, for distrubuting the load in future


#### Features:
Registration:
    POST: api/user
    Request Body params(in JSON): 
    * id
    * firstName
    * lastName
    * email
    * isGoogle
    * isFacebook
    * googleUniqueID
    * facebookUniqueID
    Response:
    Status Code: 200/201
    Response(in JSON):
    status: "Successfully created a user"
    error : nil
    
      

Login:
    GET: api/user/{id}?isGoogle=0&isFacebook=1
    Response Params:
    * id
    * firstName
    * lastName
    * email
    * isGoogle
    * isFacebook
    * googleUniqueID
    * facebookUniqueID

Record user symptoms:
    POST: api/user/symptoms
    Request body in JSON :
    * Number_of_times_pregnant
    * Plasma_glucose_test_result
    * Diastolic_blood_pressure
      
    


