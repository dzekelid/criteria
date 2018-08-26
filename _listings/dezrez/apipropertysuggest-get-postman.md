{
  "info": {
    "name": "Dezrez Search for properties/addresses that match the specified search criteria",
    "_postman_id": "95c12945-03f0-4191-b0d9-dce52d428f8d",
    "description": "Search for properties/addresses that match the specified search criteria.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Searchproperties",
      "item": [
        {
          "id": "5f275e1f-1779-418d-975f-6c12ecdd6595",
          "name": "Property_SuggestBydataContract.queryBydataContract.pageSizeBydataContract.pageNumberBydataContract.s",
          "request": {
            "url": "http://api.dezrez.com/api/property/suggest?dataContract.pageNumber=%7B%7D&dataContract.pageSize=%7B%7D&dataContract.query=%7B%7D&dataContract.suggestType=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
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
            "description": "Search for properties/addresses that match the specified search criteria."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1168a159-2f41-450e-94ac-e9db22041033"
            }
          ]
        }
      ]
    }
  ]
}