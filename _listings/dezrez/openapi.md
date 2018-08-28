swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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
  /api/group/{id}/deletesearch/{searchingRoleId}:
    delete:
      summary: Deletes Search Criteria from a Group
      description: Deletes search criteria from a group.
      operationId: Group_DeleteSearchByidBysearchingRoleId
      x-api-path-slug: apigroupiddeletesearchsearchingroleid-delete
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: searchingRoleId
        description: The id of the searching role to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Search
      - Criteria
      - From
      - Group
  /api/property/suggest:
    get:
      summary: Search for properties/addresses that match the specified search criteria
      description: Search for properties/addresses that match the specified search
        criteria.
      operationId: Property_SuggestBydataContract.queryBydataContract.pageSizeBydataContract.pageNumberBydataContract.s
      x-api-path-slug: apipropertysuggest-get
      parameters:
      - in: query
        name: dataContract.pageNumber
      - in: query
        name: dataContract.pageSize
      - in: query
        name: dataContract.query
      - in: query
        name: dataContract.suggestType
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Searchproperties
      - Addresses
      - That
      - Match
      - Specified
      - Search
      - Criteria
  /api/role/suggest:
    get:
      summary: Search for property marketing roles that match the specified search
        criteria
      description: Search for property marketing roles that match the specified search
        criteria.
      operationId: Role_SuggestBydataContract.isOnMarketBydataContract.pageNumberBydataContract.pageSizeBydataContract.
      x-api-path-slug: apirolesuggest-get
      parameters:
      - in: query
        name: dataContract.isOnMarket
      - in: query
        name: dataContract.pageNumber
      - in: query
        name: dataContract.pageSize
      - in: query
        name: dataContract.query
      - in: query
        name: dataContract.roleType
      - in: query
        name: dataContract.suggestType
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Searchproperty
      - Marketing
      - Roles
      - That
      - Match
      - Specified
      - Search
      - Criteria
  /api/simplepropertyrole/search:
    post:
      summary: Performs a searh using the specified criteria
      description: Performs a searh using the specified criteria.
      operationId: SimplePropertyRole_SearchBycriteria
      x-api-path-slug: apisimplepropertyrolesearch-post
      parameters:
      - in: body
        name: criteria
        description: The criteria
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Performs
      - Searh
      - Using
      - Specified
      - Criteria
  /api/tenancy/suggest:
    get:
      summary: Search for tenancies/tennets/landlords that match the specified search
        criteria
      description: Search for tenancies/tennets/landlords that match the specified
        search criteria.
      operationId: Tenancy_SuggestBydataContract.queryBydataContract.pageSizeBydataContract.pageNumber
      x-api-path-slug: apitenancysuggest-get
      parameters:
      - in: query
        name: dataContract.pageNumber
      - in: query
        name: dataContract.pageSize
      - in: query
        name: dataContract.query
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Searchtenancies
      - Tennets
      - Landlords
      - That
      - Match
      - Specified
      - Search
      - Criteria