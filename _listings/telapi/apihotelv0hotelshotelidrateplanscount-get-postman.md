{
  "info": {
    "name": "hetras Hotel API Version 0 Get the count of all rateplans in the hotel matching the given filter criteria.",
    "_postman_id": "758afca7-a8bc-4e67-8c09-38f1d9bbbb5c",
    "description": "Get the count of all rateplans in the hotel matching the given filter criteria..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Count",
      "item": [
        {
          "id": "630597f0-5171-4722-8799-54fc2357a1f3",
          "name": "RatePlans_GetRateplansCount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.hetras-certification.net",
              "path": [
                "api/hotel/v0/hotels/:hotelId/rateplans/$count"
              ],
              "query": [
                {
                  "key": "baseRateplan",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "channelCode",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "channelGroup",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "commissionable",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "group",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "includedServices",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "marketCodes",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "roomTypes",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sellingStatus",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "hotelId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "App-Id",
                "value": "{}",
                "description": "Application identifier",
                "disabled": false
              },
              {
                "key": "App-Key",
                "value": "{}",
                "description": "Application key",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the count of all rateplans in the hotel matching the given filter criteria.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4625036f-673e-4770-86b2-53d191ddcafb"
            }
          ]
        }
      ]
    }
  ]
}