{
  "info": {
    "name": "hetras Hotel API Version 0 Get a list of rateplans for the specified hotel id matching the filter criteria.",
    "_postman_id": "778dfda7-e88a-4c11-b01e-919e884a393d",
    "description": "With this call you can find rateplans for a hotel by different filters. By default and without any filter criteria\r\n            defined it will return you all active rateplans.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Folder",
      "item": [
        {
          "id": "d29a11fb-6594-4e08-9412-774f7e38b04a",
          "name": "Hotels_GetHotels",
          "request": {
            "url": "http://api.hetras-certification.net/api/hotel/v0/hotels",
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
            "description": "Get a list of all the hotels of a chain your application has access to.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bdd4aa5c-bb34-4b47-91f4-2cd60b41c65d"
            }
          ]
        }
      ]
    },
    {
      "name": "Details",
      "item": [
        {
          "id": "0a5cabe3-f841-48f7-b342-6f581f3ba073",
          "name": "Hotels_GetHotel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.hetras-certification.net",
              "path": [
                "api/hotel/v0/hotels/:hotelId"
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
            "description": "Get the details of the hotel with the speccified hotel id.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64a11bac-04df-44ad-b6bd-b947ee2cedf2"
            }
          ]
        }
      ]
    },
    {
      "name": "Codesthe",
      "item": [
        {
          "id": "0011b2f9-1367-49c3-8d3e-f8bd56bed139",
          "name": "Codes_GetCodes",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.hetras-certification.net",
              "path": [
                "api/hotel/v0/hotels/:hotelId/codes"
              ],
              "query": [
                {
                  "key": "code",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
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
            "description": "With this call you can find codes for a hotel by type or code. By default and without any filter criteria\r\n            defined it will return you all available codes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1922a09e-3e7a-42c8-9e1b-07771446cbd5"
            }
          ]
        }
      ]
    },
    {
      "name": "Detailsa",
      "item": [
        {
          "id": "239fe7c9-2c9b-48b6-bae6-5d44e49bf92e",
          "name": "Codes_GetCode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.hetras-certification.net",
              "path": [
                "api/hotel/v0/hotels/:hotelId/codes/:id"
              ],
              "variable": [
                {
                  "id": "hotelId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
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
            "description": "Read the details about a specific code available for the defined hotel."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0b89831-8cf5-453d-bac5-67d09f4081e2"
            }
          ]
        }
      ]
    },
    {
      "name": "Rateplansthe",
      "item": [
        {
          "id": "1ec15878-dca0-40f4-a953-9d9111703874",
          "name": "RatePlans_GetRateplans",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.hetras-certification.net",
              "path": [
                "api/hotel/v0/hotels/:hotelId/rateplans"
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
                  "key": "inlinecount",
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
                },
                {
                  "key": "skip",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "top",
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
            "description": "With this call you can find rateplans for a hotel by different filters. By default and without any filter criteria\r\n            defined it will return you all active rateplans."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "474b3c15-8d14-451a-9f81-8baff79e72fe"
            }
          ]
        }
      ]
    }
  ]
}