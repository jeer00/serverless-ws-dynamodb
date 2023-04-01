# Offline Serverless Websocket W/ dynamoDB

    This is a showcase of how to run 
    * WebsocketAPI 
    * DynamoDB
    * APIGateway (?)
    offline.
## To get started: 
* yarn
    - Change downloadurl in: node_modules/dynamodb-localhost/dynamodb/config.json to https://s3.us-west-2.amazonaws.com/dynamodb-local/dynamodb_local_latest.tar.gz]and change the import for http in node_modules/dynamodb-localhost/dynamodb/installer.js to https (this is a open issue...) 

## Note! 
    You need Java to install and run dynamodb. (or use docker container - i have not tested this. But its supported)
* sls dynamodb install 
* sls dynamodb start 

* serverless offline
* install wscat by npm install -g wscat
* wscat -c ws://localhost:3001

## Todo: 
     I have not managed to get the gateway to send messages tho the clients propertly.