# estoreexpress-errorapi-mule

### Overview
Features: [errors] [subscriber with errorq vm] [crud /estoreexpresserror]

### Test
curl --location 'http://localhost:8081/api/ping'

curl --location 'http://localhost:8081/api/readerror'

curl --location 'http://localhost:8081/api/createerror' \
--header 'Content-Type: application/json' \
--data '{
  "errorcode": "0002",
  "errortype": "APPERROR:CLIENT_ALREADY_EXISTS",
  "errormessage": "The client with ID: test1 is already registered",
  "msgtype": "register",
  "exceptiontype": "system"
}'