---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Get category tree
  description: Gets the category tree of a category. The ID of the category must be
    specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/category_branches:
    get:
      summary: Get category trees
      description: Get category trees.
      operationId: getRestCategoryBranches
      x-api-path-slug: restcategory-branches-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of results per page
      - in: query
        name: page
        description: The requested page of results
      - in: query
        name: type
        description: The category type
      responses:
        200:
          description: OK
      tags:
      - Category
      - Trees
  /rest/category_branches/{id}:
    get:
      summary: Get category tree
      description: Gets the category tree of a category. The ID of the category must
        be specified.
      operationId: getRestCategoryBranches
      x-api-path-slug: restcategory-branchesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Category
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