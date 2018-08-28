---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Get Collection tree
  description: Get collection tree.
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/collections/tree:
    get:
      summary: Get Collection tree
      description: Get collection tree.
      operationId: V2CollectionsTreeGet
      x-api-path-slug: v2collectionstree-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Collection
      - Tree
  /v2/brands/tree:
    get:
      summary: Get a Brand tree
      description: Get a brand tree.
      operationId: V2BrandsTreeGet
      x-api-path-slug: v2brandstree-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
      - Tree
  /v2/categories/categories/tree:
    get:
      summary: Category Tree
      description: Category tree.
      operationId: V2CategoriesCategoriesTreeGet
      x-api-path-slug: v2categoriescategoriestree-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category
      - Tree
  /v2/categories/tree:
    get:
      summary: Get Categories Tree
      description: Get categories tree.
      operationId: V2CategoriesTreeGet
      x-api-path-slug: v2categoriestree-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Categories
      - Tree
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