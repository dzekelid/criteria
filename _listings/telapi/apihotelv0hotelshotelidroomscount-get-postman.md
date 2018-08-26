{
  "info": {
    "name": "hetras Hotel API Version 0 Get the count of all rooms in the hotel matching the given filter criteria.",
    "_postman_id": "790f73f7-a5a2-4790-9da7-8d1bbd7b0171",
    "description": "Get the count of all rooms in the hotel matching the given filter criteria..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Count",
      "item": [
        {
          "id": "f7d17aba-6e10-47fe-8cdf-0fa807914608",
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
              "id": "27cf65e8-5338-4b66-ba27-f72540810d57"
            }
          ]
        },
        {
          "id": "4f153077-b316-4c56-8c2c-04776b7a0d84",
          "name": "RatePlans_GetRatesCount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.hetras-certification.net",
              "path": [
                "api/hotel/v0/hotels/:hotelId/rateplans/:rateplanCode/rates/$count"
              ],
              "query": [
                {
                  "key": "from",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "to",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "hotelId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "rateplanCode",
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
            "description": "Get the count of all active and loaded daily rates for the defined rateplan in a specified time period.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d3a0a9b-987a-413a-a1eb-5ec5915f9770"
            }
          ]
        },
        {
          "id": "3630f662-55a7-407d-a73c-10861aed931f",
          "name": "Rooms_GetRoomsCount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.hetras-certification.net",
              "path": [
                "api/hotel/v0/hotels/:hotelId/rooms/$count"
              ],
              "query": [
                {
                  "key": "amenities",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "conditions",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "locations",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maintenances",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "occupancy",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "roomTypes",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "views",
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
            "description": "Get the count of all rooms in the hotel matching the given filter criteria.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e454fd5-0656-4c29-aace-249f733e8835"
            }
          ]
        }
      ]
    }
  ]
}