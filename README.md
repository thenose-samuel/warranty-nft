Currently, a tangible receipt or warranty card serves as the basis for determining the warranty's validity. This raises a number of issues and hereby we provide the following solutions:

1) The warranty document can be easily forged. Tokenizing the physical warranties as NFTs can come to the rescue as NFTs cannot be falsified.

2) The warranty document may not be uniform across all sellers. No matter who issued it or when, a warranty is standardized for this NFT app.

3) Warranty cards for products that have expired could be issued "under the table" by a dishonest authorized dealer. The blockchain's transaction history can be scanned, allowing us to quickly identify any malicious activity.

We have divided our problem into 3 parts, i.e,;

For Minting
For Burning
For Viewing

Here are the following block diagrams for each of the sub-problems for easier understanding:

For Minting
[![For-Minting-3.png](https://i.postimg.cc/4dXzKLrG/For-Minting-3.png)](https://postimg.cc/Lq0qwT9Q)

For Burning
[![For-Burning-1.png](https://i.postimg.cc/zGnbnwwG/For-Burning-1.png)](https://postimg.cc/87zzG6n2)
For Viewing

[![For-Viewing.png](https://i.postimg.cc/qRZzk1rj/For-Viewing.png)](https://postimg.cc/8JM14Bj6)




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
