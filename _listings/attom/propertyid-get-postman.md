{
  "info": {
    "name": "Attom Data Solutions API Returns a list of properties that fit a criteria.",
    "_postman_id": "17dea6e7-f617-4198-ab24-0be3d74354b5",
    "description": "Get a list of property IDs within a specific geography that have a specific number of beds. Use orderby to choose how you want your results sorted.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Returns",
      "item": [
        {
          "id": "7c55560c-92d3-46f6-8c50-8c9468f97bce",
          "name": "getPropertyIdList",
          "request": {
            "url": "http://search.onboard-apis.com/communityapi/v2.0.0/property/id?geoid=%7B%7D&maxBeds=%7B%7D&minBeds=%7B%7D&orderby=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "accept",
                "value": "{}",
                "description": "application/xml or application/json (default)",
                "disabled": false
              },
              {
                "key": "apikey",
                "value": "{}",
                "description": "Application Key",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of property IDs within a specific geography that have a specific number of beds. Use orderby to choose how you want your results sorted."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78aebfce-8428-4d4f-b3d3-e01598df328e"
            }
          ]
        }
      ]
    }
  ]
}