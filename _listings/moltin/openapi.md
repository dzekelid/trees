swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
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