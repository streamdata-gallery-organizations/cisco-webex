---
swagger: "2.0"
x-collection-name: Cisco WebEx
x-complete: 0
info:
  title: Webex Teams Admin API Get Events Details
  description: "Shows details for an event, by event ID.\r\nSpecify the event ID in
    the eventId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-events-eventId-get.html"
  version: 1.0.0
host: api.ciscospark.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /people/{_person}:
    get:
      summary: Get Person Details1
      description: |-
        Shows details for a person, by ID.
        Specify the person ID in the personId parameter in the URI.

        https://developer.webex.com/endpoint-people-personId-get.html
      operationId: PeopleByPersonGet2
      x-api-path-slug: people-person-get
      parameters:
      - in: path
        name: _person
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Person
      - Details1
    put:
      summary: Update a Person
      description: "Update details for a person, by ID.\r\n\r\nSpecify the person
        ID in the personId parameter in the URI. Only an admin can update a person
        details.\r\n\r\nhttps://developer.webex.com/endpoint-people-personId-put.html\r\n\r\nExample
        Request:\r\n``` json\r\n{\r\n  'emails\" : [ 'johnny.chang@foomail.com', 'jchang@barmail.com'
        ],\r\n  'displayName' : 'John Andersen',\r\n  'firstName' : 'John',\r\n  'lastName'
        : 'Andersen',\r\n  'avatar' : 'https://1efa7a94ed21783e352-c62266528714497a17239ececf39e9e2.ssl.cf1.rackcdn.com/V1~54c844c89e678e5a7b16a306bc2897b9~wx29yGtlTpilEFlYzqPKag==~1600',\r\n
        \ 'orgId' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',\r\n  'roles'
        : [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy',
        'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX'
        ],\r\n  'licenses' : [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy',
        'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX'
        ]\r\n}\r\n```"
      operationId: PeopleByPersonPut
      x-api-path-slug: people-person-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: _person
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Person
    delete:
      summary: Delete a Person
      description: |-
        Remove a person from the system. Only an admin can remove a person.

        Specify the person ID in the personId parameter in the URI.

        https://developer.webex.com/endpoint-people-personId-delete.html
      operationId: PeopleByPersonDelete
      x-api-path-slug: people-person-delete
      parameters:
      - in: path
        name: _person
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Person
  /roles:
    get:
      summary: Get roles (to fetch a role id)
      description: |-
        List all roles.

        https://developer.webex.com/endpoint-roles-get.html

        Example Response:
        ``` json
        {
          'items' : [ {
            'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',
            'displayName' : 'Full Administrator'
          } ]
        }
        ```
      operationId: RolesGet2
      x-api-path-slug: roles-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Roles
      - (to
      - Fetch
      - Role
      - Id)
  /licenses/{_license}:
    get:
      summary: Get License Details
      description: "Shows details for a license, by ID.\r\n\r\nSpecify the license
        ID in the licenseId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-licenses-licenseId-get.html\r\n\r\nExample
        Response:\r\n``` json\r\n{\r\n  'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',\r\n
        \ 'displayName' : 'Spark Calling',\r\n  'totalUnits' : '42',\r\n  'consumedUnits'
        : \"8'\r\n}\r\n```"
      operationId: LicensesByLicenseGet
      x-api-path-slug: licenses-license-get
      parameters:
      - in: path
        name: _license
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - License
      - Details
  /roles/{_role}:
    get:
      summary: Get Role Details
      description: |-
        Shows details for a role, by ID.

        Specify the role ID in the roleId parameter in the URI.

        https://developer.webex.com/endpoint-roles-roleId-get.html

        Example Response:
        ``` json
        {
          'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',
          'displayName' : 'Full Administrator'
        }
        ```
      operationId: RolesByRoleGet
      x-api-path-slug: roles-role-get
      parameters:
      - in: path
        name: _role
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Role
      - Details
  /people/me:
    get:
      summary: Get Person Details (me)
      description: |-
        Show the profile for the authenticated user.

        https://developer.webex.com/endpoint-people-me-get.html
      operationId: PeopleMeGet
      x-api-path-slug: peopleme-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Person
      - Details
      - (me)
  /events:
    get:
      summary: List Events (new messages)
      description: |-
        List events in your organization. Several query parameters are available to filter the response.
        Long result sets will be split into pages.

        https://developer.webex.com/endpoint-events-get.html
      operationId: EventsGet4
      x-api-path-slug: events-get
      parameters:
      - in: query
        name: resource
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Events
      - (new
      - Messages)
  /licenses:
    get:
      summary: List Licenses
      description: |-
        List all licenses for a given organization. If no orgId is specified, the default is the organization of the authenticated user.

        https://developer.webex.com/endpoint-licenses-get.html

        Example of a response:
        ``` json
        {
          'items' : [ {
            'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',
            'displayName' : 'Spark Calling',
            'totalUnits' : '42',
            'consumedUnits' : '8'
          } ]
        }
        ```
      operationId: LicensesGet
      x-api-path-slug: licenses-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Licenses
  /events/{_event}:
    get:
      summary: Get Events Details
      description: "Shows details for an event, by event ID.\r\nSpecify the event
        ID in the eventId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-events-eventId-get.html"
      operationId: EventsByEventGet
      x-api-path-slug: events-event-get
      parameters:
      - in: path
        name: _event
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Events
      - Details
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