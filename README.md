#Set up details

execute the following 

1. `npm i`
2. `npm start`

the following apis are used to interact with the backend on localhost

`curl --location --request GET 'http://localhost:3000/viewWarrantyTokens/?walletAddress=[customer's wallet address]`

`curl --location --request POST 'http://localhost:3000/createWarrantyToken' \
--header 'Content-Type: application/json' \
--data-raw '{
    "productId": "123",
    "walletAddress": "456",
    "warrantyDetails": "hello world",
    "issueDate": "23-45-2001",
    "expirationDate": "06-09-2001"
}'`
