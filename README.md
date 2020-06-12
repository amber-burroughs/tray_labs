
**Base URL**: https://2b1011ad-6240-4dc9-ae58-284faaa14e80.trayapp.io
**Methods:** none

**GET**

    {
        "message": "Uh-Oh! I do not know the endpoint you provided 😥",
        "endpoint": "/v1/",
        "incorrect" endpoint: "/",
        "method": "GET"
    }

**POST**

    {
        "message": "Oops! Please provide the proper endpoint 😥",
        "endpoint": "/v1/people/",
        "method": "POST"
    }

**Endpoint: 
/v1/**
- Practice making an API request
Methods: GET

**GET /v1/**

**RESPONSE**

    {
        "message": "Great job using the GET Method! 🎉",
        "Method": "GET",
        "Endpoint": "/v1/"
    }

**POST /v1/**

    {
        "message": "Oops! Please provide the proper endpoint 😥",
        "endpoint": "/v1/people/",
        "method": "POST"
    }

**Endpoint: 
/v1/people/**
- Practice making an API request
- Request all people data
- Submit a new person

**Methods: GET, POST**

**GET /v1/people/**

**RESPONSE**

    {
        "message": "Woo-hoo! You hit an API endpoint 😎",
        "data": [
            {
                "key": "amber",
                "created": "2020-06-12T10:44:52.976Z"
            }
        ],
        "method": "GET",
        "endpoint": "/v1/people/"
    }

**POST  /v1/people/**

    {
        "name": "amber hernandez",
        "food":"pizza",
        "company":"Tray.io"
    }

**RESPONSE**

    {
        "message": "Great job using the POST Method! 👏",
        "queryParam": "amber-hernandez",
        "endpoint": "/v1/people/",
        "route": "amber-hernandez",
        "method": "POST"
    }

**Route
/v1/people/:name**
- Practice making an API request
- Request people data for a particular person with their name route
- Name routes are create when data is sent to the API
- If a POST request is made using a name route the route will be ignored

**Methods: GET, POST**

**GET /v1/people/:name**

**RESPONSE**

    {
        "message": "AWESOME! You hit an API endpoint and uses a route 🤩",
        "data": "Amber",
        "endpoint": "/v1/people/",
        "route": "amber",
        "method": "GET"
    }

**POST /v1/people/:name**

    {
        "name": "Tray Labs",
        "food":"Grilled Cheese",
        "company":"Tray.io",
        "role": "Customer enablement"
    }

**RESPONSE**

    {
        "message": "Great job using the POST Method! 👏",
        "queryParam": "tray-labs",
        "endpoint": "/v1/people/",
        "route": "tray-labs",
        "method": "POST"
    }


**Query Parameter
/v1/people?name=:your-generated-route**
- Request people data for a particular person with their name route as query parameter
- Name routes are create when data is sent to the API
- If a POST request is made using query parameters the params will be ignored
Methods: GET,

**GET /v1/people?name=:your-generated-route**

**RESPONSE**

    {
        "message": "Amazing! You hit an API endpoint and uses a query parameter 👍",
        "data": {
            "endpoint": "tray-labs",
            "role": "Customer enablement",
            "name": "Tray Labs",
            "company": "Tray.io",
            "food": "Grilled Cheese"
        },
        "endpoint": "/v1/people/",
        "method": "GET",
        "query param": {
            "name": "tray-labs"
        }
    }

**POST /v1/people?name=:your-generated-route**

    {
        "message": "Great job using the POST Method! 👏",
        "queryParam": "tray-labs",
        "endpoint": "/v1/people/",
        "route": "tray-labs",
        "method": "POST"
    }

**RESPONSE**

    {
        "message": "Great job using the POST Method! 👏",
        "queryParam": "tray-labs",
        "endpoint": "/v1/people/",
        "route": "tray-labs",
        "method": "POST"
    }


**Status Codes:**

 - **200** - Success 
 - **404** - Failure | Resource not found


