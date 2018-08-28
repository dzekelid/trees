swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
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