# airalo-api-test
API test for Airalo Partner API
# Postman API Test Collection

This repository contains 2 Postman collections and 1 postman enviornment for Airalo API test. 

## Files

airalo-api-test/Collection1.postman_collection.json
airalo-api-test/Collection2.postman_collection.json
  → Contains the API test cases.

airalo-api-test/Airalo API Test.postman_environment.json
  → Used for environment variables like base URL, tokens, etc.

## How to Use

## 1. Import into Postman

1. Open Postman.
2. Click **Import**.
3. Select the Collection1.postman_collection.json & Collection2.postman_collection.json file.
4. Import the environment file too.

## 2. Run the Collection1

- Open the imported Collection1 file in Postman.
- Select the environment Airalo API Test
- Test_Case_1 - Run 'POST Auth token' request to generate a token, API will return a 200 OK HTTP response
- Test_Case_2 - Run 'POST Submit Order' request to POST an order for 6 "merhaba-7days-1gb" eSIMs,  API will return a 200 OK HTTP response
- Test_Case_3 - Run 'GET Get a list of sim' request to query for list of 6 "merhaba-7days-1gb" eSIMs,  API will return a 200 OK HTTP response
- For order details and eSIM properties, response body can be checked below the order screen

## 3. Automated test by using run command

- Open the imported Collection2 file in Postman.
- Select the environment Airalo API Test
- Test_Case_1 - Run all the three test together by using run command in Collection2. Provide the iterations as 1 and delay as 0 ms.
- Verify 200 OK reponse for all the requests together.
- For order details and eSIM properties, response body can be checked by clicking on each request individually.

## 4. Tools Used

- [Postman](https://www.postman.com/)

