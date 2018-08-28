---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Saves Lettings Search Criteria to a group
  version: 1.0.0
  description: Saves lettings search criteria to a group.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/group/{id}/savesalessearch:
    post:
      summary: Saves Search Criteria to a Group
      description: Saves search criteria to a group.
      operationId: Group_SaveSalesSearchByidBysearchDataContract
      x-api-path-slug: apigroupidsavesalessearch-post
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: searchDataContract
        description: The groups search criteria
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Saves
      - Search
      - Criteria
      - To
      - Group
  /api/group/{id}/savelettingssearch:
    post:
      summary: Saves Lettings Search Criteria to a group
      description: Saves lettings search criteria to a group.
      operationId: Group_SaveLettingsSearchByidBysearchingDataContract
      x-api-path-slug: apigroupidsavelettingssearch-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: searchingDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Saves
      - Lettings
      - Search
      - Criteria
      - To
      - Group
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---