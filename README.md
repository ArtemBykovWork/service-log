# Service Log

## Description
`service-log` is a microservice that provides an API to log request objects. This service is intended to be used by other microservices to log their requests.

## API Endpoints
### POST /log
- **Description**: Logs the received request object to the console.
- **Request**: JSON object representing the request to be logged.
- **Response**: JSON object confirming the log.
- **Example**:
  ```json
  // Request
  {
    "number": 5,
    "shuffledArray": [4, 2, 1, 5, 3]
  }
  // Response
  {
    "status": "logged"
  }