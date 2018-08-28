swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/drive/special/{name}:
    get:
      summary: Get A Special Folder By Name
      description: Get a special folder by name Use the special collection to access
        a special folder by name.
      operationId: GetASpecialFolderByName
      x-api-path-slug: medrivespecialname-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Special
      - FolderName