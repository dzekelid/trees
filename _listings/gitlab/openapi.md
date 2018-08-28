swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/repository/tree:
    get:
      summary: Get Projects Repository Tree
      description: Get a project repository tree
      operationId: getV3ProjectsIdRepositoryTree
      x-api-path-slug: v3projectsidrepositorytree-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: path
        description: The path of the tree
      - in: query
        name: recursive
        description: Used to get a recursive tree
      - in: query
        name: ref_name
        description: The name of a repository branch or tag, if not given the default
          branch is used
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
      - Tree