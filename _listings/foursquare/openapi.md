swagger: "2.0"
x-collection-name: Foursquare
x-complete: 1
info:
  title: Foursquare
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
  /specials/search:
    get:
      summary: Get Specials Search
      description: /specials/list
      operationId: specialslist
      x-api-path-slug: specialssearch-get
      parameters:
      - in: query
        name: alt
        description: Altitude of the users location, in meters
      - in: query
        name: altAcc
        description: Accuracy of the users altitude, in meters
      - in: query
        name: limit
        description: Number of results to return, up to 50
      - in: query
        name: ll
        description: Latitude and longitude to search near
      - in: query
        name: llAcc
        description: Accuracy of latitude and longitude, in meters
      - in: query
        name: radius
        description: Limit results to venues within this many meters of the specified
          location
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Specials
      - Search
  /specials/{ID}/flag:
    post:
      summary: Post Specials Flag
      description: /specials/{SPECIAL_ID}/configuration
      operationId: specialsspecial-idconfiguration
      x-api-path-slug: specialsidflag-post
      parameters:
      - in: query
        name: ID
        description: The id of the special being flagged
      - in: path
        name: ID
      - in: query
        name: problem
        description: One of not_redeemable, not_valuable, other
      - in: query
        name: text
        description: Additional text about why the user has flagged this special
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: The id of the venue running the special
      responses:
        200:
          description: OK
      tags:
      - Specials
      - Flag
  /specials/{SPECIAL_ID}:
    get:
      summary: Get Specials
      description: /settings/{SETTING_ID}/set
      operationId: settingssetting-idset
      x-api-path-slug: specialsspecial-id-get
      parameters:
      - in: query
        name: SPECIAL_ID
        description: ID of special to retrieve
      - in: path
        name: SPECIAL_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: ID of a venue the special is running at
      responses:
        200:
          description: OK
      tags:
      - Specials
  /specials/{SPECIAL_ID}/configuration:
    get:
      summary: Get Specials Configuration
      description: /specials/search
      operationId: specialssearch
      x-api-path-slug: specialsspecial-idconfiguration-get
      parameters:
      - in: query
        name: SPECIAL_ID
        description: The ID of the special to retrieve configuration details for
      - in: path
        name: SPECIAL_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Specials
      - Configuration
  /specials/{SPECIAL_ID}/retire:
    post:
      summary: Post Specials Retire
      description: /specials/{ID}/flag
      operationId: specialsidflag
      x-api-path-slug: specialsspecial-idretire-post
      parameters:
      - in: query
        name: SPECIAL_ID
        description: The ID of the special to retire
      - in: path
        name: SPECIAL_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Specials
      - Retire