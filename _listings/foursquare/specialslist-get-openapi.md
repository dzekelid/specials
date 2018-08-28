---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Get Specials List
  description: /specials/add
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /specials/add:
    post:
      summary: Post Specials Add
      description: /specials/{SPECIAL_ID}
      operationId: specialsspecial-id
      x-api-path-slug: specialsadd-post
      parameters:
      - in: query
        name: cost
        description: The amount of money the user must spend to use this special in
          dollars and cents
      - in: query
        name: count1
        description: Count for frequency, count, regular, swarm, friends, and flash
          specials
      - in: query
        name: count2
        description: Secondary count for regular, flash specials
      - in: query
        name: count3
        description: Tertiary count for flash specials
      - in: query
        name: finePrint
        description: Maximum length of 200 characters
      - in: query
        name: name
        description: A name for the special
      - in: query
        name: offerId
        description: Maximum length of 16 characters
      - in: query
        name: text
        description: Maximum length of 200 characters
      - in: query
        name: type
        description: The type of special
      - in: query
        name: unlockedText
        description: Maximum length of 200 characters
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Specials
  /specials/list:
    get:
      summary: Get Specials List
      description: /specials/add
      operationId: specialsadd
      x-api-path-slug: specialslist-get
      parameters:
      - in: query
        name: status
        description: 'Which specials to return: pending, active, expired, all'
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: Comma-separated list of venue IDs; filters results to the specials
          assigned to the venue(s)
      responses:
        200:
          description: OK
      tags:
      - Specials
      - List
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