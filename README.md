### Authentication  API

#### Prerequisite
1.nodejs
2.mysql

#### To run the API in local, run the below commands from the root folder of the project
1.npm install
2.npm start

#### Endpoints exposed

1.Login(/user/signin)
2.Signup(/user/signup)
3.welcome(/user/welcome)
4.logout(/user/logout)

#### To test the API using Postman, please find the curl request for all the four end points below

#### Login
curl -X POST \
  http://localhost:9000/user/signin \
  -H 'cache-control: no-cache' \
  -H 'content-type: application/json' \
  -H 'postman-token: 1208e8e2-bc44-ea3f-1e8f-6ef618c7ccb0' \
  -d '{
    "username": "Prakash",
    "email": "1234@gmail.com",
    "password": "1234"
}'

#### Sign UP

curl -X POST \
  http://localhost:9000/user/signup \
  -H 'cache-control: no-cache' \
  -H 'content-type: application/json' \
  -H 'postman-token: 98e0be16-4660-38c4-9cb1-fa623c12d12b' \
  -d '{
    "username": "Prakash",
    "email": "1234@gmail.com",
    "password": "1234",
    "name": "Chandra Prakash"
}'

#### Welcome User

curl -X GET \
  http://localhost:9000/user/welcome \
  -H 'authorization: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6OSwiaWF0IjoxNjQzNjcyNTU4LCJleHAiOjE2NDM5MzE3NTh9.OoLc8Y2LzL083HzM_RRlcL6MMJyyfCfKmVDb_iLYTwg' \
  -H 'cache-control: no-cache' \
  -H 'content-type: application/json'

#### Logout User

curl -X GET \
  http://localhost:9000/user/logout \
  -H 'authorization: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6OSwiaWF0IjoxNjQzNjcyNTU4LCJleHAiOjE2NDM5MzE3NTh9.OoLc8Y2LzL083HzM_RRlcL6MMJyyfCfKmVDb_iLYTwg' \
  -H 'cache-control: no-cache'
