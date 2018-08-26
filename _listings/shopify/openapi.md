---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/customer_saved_searches/1189248515/customers.json:
    get:
      summary: Get all customers who match the criteria
      description: Get all customers who match the criteria.
      operationId: getAdminCustomerSavedSearches1189248515Customers.json
      x-api-path-slug: admincustomer-saved-searches1189248515customers-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Customers
      - Who
      - Match
      - Criteria
---