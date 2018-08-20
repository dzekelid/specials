---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Remove special arrangements from a property
  version: 1.0.0
  description: Remove special arrangements from a property.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/property/{id}/specialarrangements:
    get:
      summary: Get a list of special arrangements for a property
      description: Get a list of special arrangements for a property.
      operationId: Property_SpecialArrangementsByid
      x-api-path-slug: apipropertyidspecialarrangements-get
      parameters:
      - in: path
        name: id
        description: The Id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Special
      - Arrangementsa
      - Property
  /api/property/{id}/specialarrangements/add:
    post:
      summary: Add special arrangements for a property
      description: Add special arrangements for a property.
      operationId: Property_AddSpecialArrangementsByidByarrangementsToAdd
      x-api-path-slug: apipropertyidspecialarrangementsadd-post
      parameters:
      - in: body
        name: arrangementsToAdd
        description: A collection of arrangements codes to add
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Special
      - Arrangementsa
      - Property
  /api/property/{id}/specialarrangements/remove:
    delete:
      summary: Remove special arrangements from a property
      description: Remove special arrangements from a property.
      operationId: Property_RemoveSpecialArrangementsByidByarrangementIds
      x-api-path-slug: apipropertyidspecialarrangementsremove-delete
      parameters:
      - in: query
        name: arrangementIds
        description: The ids of the special arrangements to remove
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Special
      - Arrangements
      - From
      - Property
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