---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get User Assigned Product Catalogs
  description: User Assigned Product Catalogs
  termsOfService: https://www.facebook.com/policies/
  version: 1.0.0
host: graph.facebook.com
basePath: /v3.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /&#123;user-id&#125;/assigned_product_catalogs:
    get:
      summary: Get User Assigned Product Catalogs
      description: User Assigned Product Catalogs
      operationId: getUserAssignedProductCatalogs
      x-api-path-slug: 123userid125assigned-product-catalogs-get
      parameters:
      - in: query
        name: access_typestring
        description: Checks if business has owner or agency access on the asset
        type: string
      - in: query
        name: permitted_rolesliststring
        description: Roles that are assignable on this object
        type: string
      - in: query
        name: rolestring
        description: Role of this particular user on this object
        type: string
      - in: query
        name: roles_and_tasksliststring
        description: All unpacked roles of this particular user on this object
        type: string
      responses:
        200:
          description: OK
      tags:
      - User
      - Assigned
      - Product
      - Catalogs
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