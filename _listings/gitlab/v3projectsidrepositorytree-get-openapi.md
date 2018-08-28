---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Get Projects Repository Tree
  version: 1.0.0
  description: Get a project repository tree
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