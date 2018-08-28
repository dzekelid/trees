swagger: "2.0"
x-collection-name: BigCommerce
x-complete: 1
info:
  title: BigCommerce API V3
  description: collection-of-requests-for-interacting-with-bigcommerces-v3-api
  version: 1.0.0
host: api.bigcommerce.com
basePath: /stores
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{store_hash}/v3/catalog/categories/tree:
    get:
      summary: Retrieve category structure/tree
      description: ""
      operationId: V3CatalogCategoriesTreeByStoreHashGet
      x-api-path-slug: store-hashv3catalogcategoriestree-get
      parameters:
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Category
      - Structure
      - Tree