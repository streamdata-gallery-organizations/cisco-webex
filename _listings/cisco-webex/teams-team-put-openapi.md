---
swagger: "2.0"
x-collection-name: Cisco WebEx
x-complete: 0
info:
  title: WebEx Teams API Update a team
  description: |-
    Update a team.

    https://developer.webex.com/endpoint-teams-teamId-put.html
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
      summary: Get person details (me)
      description: |-
        Show the profile for the authenticated user.

        https://developer.webex.com/endpoint-people-me-get.html
      operationId: PeopleMeGet
      x-api-path-slug: peopleme-get
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
  /organizations:
    get:
      summary: List Organizations
      description: |-
        List all organizations visible by your account.

        https://developer.webex.com/endpoint-organizations-get.html

        Example Response:
        ``` json
        {
          'items' : [ {
            'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',
            'displayName' : 'Acme, Inc.',
            'created' : '2015-10-18T14:26:16+00:00'
          } ]
        }
        ```
      operationId: OrganizationsGet
      x-api-path-slug: organizations-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Organizations
  /people:
    get:
      summary: List people (whose name starts with)
      description: |-
        List people in your organization.

        https://developer.webex.com/endpoint-people-get.html
      operationId: PeopleGet2
      x-api-path-slug: people-get
      parameters:
      - in: query
        name: displayName
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - People
      - (whose
      - Name
      - Starts
      - With)
    post:
      summary: Create a Person (random)
      description: |-
        Create a new user account for a given organization. Only an admin can create a new user account.

        https://developer.webex.com/endpoint-people-post.html

        Example Request:
        ``` json
        {
          'emails' : [ 'johnny.chang@foomail.com', 'jchang@barmail.com' ],
          'displayName' : 'John Andersen',
          'firstName' : 'John',
          'lastName' : 'Andersen',
          'avatar' : 'https://1efa7a94ed21783e352-c62266528714497a17239ececf39e9e2.ssl.cf1.rackcdn.com/V1~54c844c89e678e5a7b16a306bc2897b9~wx29yGtlTpilEFlYzqPKag==~1600',
          'orgId' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',
          'roles' : [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy', 'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX' ],
          'licenses' : [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy', 'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX' ]
        }

        Example Response:
        {
          'id' : 'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mNWIzNjE4Ny1jOGRkLTQ3MjctOGIyZi1mOWM0NDdmMjkwNDY',
          'emails' : [ 'johnny.chang@foomail.com', 'jchang@barmail.com' ],
          'displayName' : 'John Andersen',
          'firstName' : 'John',
          'lastName' : 'Andersen',
          'avatar' : 'https://1efa7a94ed21783e352-c62266528714497a17239ececf39e9e2.ssl.cf1.rackcdn.com/V1~54c844c89e678e5a7b16a306bc2897b9~wx29yGtlTpilEFlYzqPKag==~1600',
          'orgId' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',
          'roles' : [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy', 'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX' ],
          'licenses' : [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy', 'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX' ],
          'created' : '2015-10-18T14:26:16+00:00',
          'timezone' : 'America/Denver'
        }
        ```
      operationId: PeoplePost
      x-api-path-slug: people-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Person
      - (random)
  /organizations/{_organization}:
    get:
      summary: Get Organization Details
      description: "Shows details for an organization, by ID.\r\n\r\nSpecify the org
        ID in the orgId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-organizations-orgId-get.html\r\n\r\nExample
        Response:\r\n``` json\r\n{\r\n  'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',\r\n
        \ 'displayName' : 'Acme, Inc.',\r\n  'created' : '2015-10-18T14:26:16+00:00'\r\n}\r\n```"
      operationId: OrganizationsByOrganizationGet
      x-api-path-slug: organizations-organization-get
      parameters:
      - in: path
        name: _organization
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Organization
      - Details
  /webhooks:
    get:
      summary: List webhooks
      description: |-
        Lists all of your webhooks.

        https://developer.webex.com/endpoint-webhooks-get.html
      operationId: WebhooksGet
      x-api-path-slug: webhooks-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Webhooks
    post:
      summary: Create a webhook (all events, all rooms)
      description: |-
        Creates a webhook for messages/created event.

        Note that you'll need to change the requestb.in URI to your own to see the webhook in action.

        https://developer.webex.com/endpoint-webhooks-post.html
      operationId: WebhooksPost
      x-api-path-slug: webhooks-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Webhook
      - (all
      - Events
      - ""
      - ""
      - Rooms)
  /rooms:
    get:
      summary: List rooms
      description: "List rooms.\r\n\r\nBy default, lists rooms to which the authenticated
        user belongs.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-get.html"
      operationId: RoomsGet3
      x-api-path-slug: rooms-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Rooms
    post:
      summary: Create a Team room
      description: |-
        Creates a room. The authenticated user is automatically added as a member of the room. See the Memberships API to learn how to add more people to the room.

        https://developer.webex.com/endpoint-rooms-post.html
      operationId: RoomsPost5
      x-api-path-slug: rooms-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Room
  /memberships/{_membership}:
    get:
      summary: Get membership details
      description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
        ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-memberships-membershipId-get.html"
      operationId: MembershipsByMembershipGet
      x-api-path-slug: memberships-membership-get
      parameters:
      - in: path
        name: _membership
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Membership
      - Details
    put:
      summary: Update a membership
      description: |-
        Updates properties for a membership by ID.

        Specify the membership ID in the membershipId URI parameter.

        https://developer.ciscospark.com/endpoint-memberships-membershipId-put.html
      operationId: MembershipsByMembershipPut
      x-api-path-slug: memberships-membership-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: _membership
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Membership
    delete:
      summary: Delete membership
      description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in
        the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-memberships-membershipId-delete.html"
      operationId: MembershipsByMembershipDelete
      x-api-path-slug: memberships-membership-delete
      parameters:
      - in: path
        name: _membership
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Membership
  /messages/{_message}:
    get:
      summary: Get message details
      description: |-
        Shows details for a message, by message ID.

        Specify the message ID in the messageId parameter in the URI.

        https://developer.webex.com/endpoint-messages-messageId-get.html
      operationId: MessagesByMessageGet
      x-api-path-slug: messages-message-get
      parameters:
      - in: path
        name: _message
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Message
      - Details
    delete:
      summary: Delete a message
      description: |-
        Deletes a message, by message ID.

        Specify the message ID in the messageId parameter in the URI.

        https://developer.webex.com/endpoint-messages-messageId-delete.html
      operationId: MessagesByMessageDelete
      x-api-path-slug: messages-message-delete
      parameters:
      - in: path
        name: _message
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Message
  /messages:
    get:
      summary: List messages
      description: "Lists all messages in a room. If present, includes the associated
        media content attachment for each message.\r\n\r\nThe list sorts the messages
        in descending order by creation date.\r\n\r\nhttps://developer.webex.com/endpoint-messages-get.html"
      operationId: MessagesGet
      x-api-path-slug: messages-get
      parameters:
      - in: query
        name: roomId
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Messages
    post:
      summary: Create a message (html)
      description: |-
        HTML is not officially supported by the API, but will work in some cases

        To get more info about message formatting, check https://developer.ciscospark.com/formatting-messages.html

        https://developer.webex.com/endpoint-messages-post.html
      operationId: MessagesPost11
      x-api-path-slug: messages-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Message
      - (html)
  /rooms/{_room}:
    get:
      summary: Get Team room details
      description: "Shows details for a room, by ID.\r\n\r\nSpecify the room ID in
        the roomId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-roomId-get.html"
      operationId: RoomsByRoomGet2
      x-api-path-slug: rooms-room-get
      parameters:
      - in: path
        name: _room
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Room
      - Details
    put:
      summary: Update a room
      description: "Updates details for a room, by ID.\r\n\r\nSpecify the room ID
        in the roomId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-roomId-put.html"
      operationId: RoomsByRoomPut2
      x-api-path-slug: rooms-room-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: _room
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Room
    delete:
      summary: Delete a Team room
      description: "Deletes a room, by ID.\r\n\r\nSpecify the room ID in the roomId
        parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-roomId-delete.html"
      operationId: RoomsByRoomDelete5
      x-api-path-slug: rooms-room-delete
      parameters:
      - in: path
        name: _room
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Room
  /teams:
    get:
      summary: List teams
      description: |-
        List teams.

        https://developer.webex.com/endpoint-teams-get.html
      operationId: TeamsGet
      x-api-path-slug: teams-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Teams
    post:
      summary: Create a team
      description: |-
        Create a new team.

        https://developer.webex.com/endpoint-teams-post.html
      operationId: TeamsPost2
      x-api-path-slug: teams-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
  /webhooks/{_webhook}:
    get:
      summary: Get webhook details1
      description: "Shows details for a webhook, by ID.\r\n\r\nSpecify the webhook
        ID in the webhookId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-webhooks-webhookId-get.html"
      operationId: WebhooksByWebhookGet2
      x-api-path-slug: webhooks-webhook-get
      parameters:
      - in: path
        name: _webhook
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Webhook
      - Details1
    put:
      summary: Update a webhook
      description: "Updates a webhook, by ID.\r\n\r\nSpecify the webhook ID in the
        webhookId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-webhooks-webhookId-put.html"
      operationId: WebhooksByWebhookPut
      x-api-path-slug: webhooks-webhook-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: _webhook
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Webhook
    delete:
      summary: Delete a webhook1
      description: "Deletes a webhook, by ID.\r\n\r\nSpecify the webhook ID in the
        webhookId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-webhooks-delete.html"
      operationId: WebhooksByWebhookDelete2
      x-api-path-slug: webhooks-webhook-delete
      parameters:
      - in: path
        name: _webhook
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Webhook1
  /memberships:
    get:
      summary: List memberships (for all rooms)
      description: |-
        Lists all room memberships. By default, lists memberships for rooms to which the authenticated user belongs.

        Use query parameters to filter the response.

        Use roomId to list memberships for a room, by ID.

        Use either personId or personEmail to filter the results.

        https://developer.webex.com/endpoint-memberships-get.html
      operationId: MembershipsGet2
      x-api-path-slug: memberships-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Memberships
      - (for
      - ""
      - Rooms)
    post:
      summary: Create a membership
      description: |-
        Add someone to a room by Person ID or email address; optionally making them a moderator.

        https://developer.webex.com/endpoint-memberships-post.html
      operationId: MembershipsPost
      x-api-path-slug: memberships-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Membership
  /team/memberships/{_membership}:
    get:
      summary: Get team membership details
      description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
        ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-get.html"
      operationId: TeamMembershipsByMembershipGet
      x-api-path-slug: teammemberships-membership-get
      parameters:
      - in: path
        name: _membership
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Membership
      - Details
    put:
      summary: Update a team membership
      description: |-
        Updates properties for a membership by ID.

        Specify the membership ID in the membershipId URI parameter.

        https://developer.webex.com/endpoint-teammemberships-membershipId-put.html
      operationId: TeamMembershipsByMembershipPut
      x-api-path-slug: teammemberships-membership-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: _membership
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Membership
    delete:
      summary: Delete a team membership
      description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in
        the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-delete.html"
      operationId: TeamMembershipsByMembershipDelete
      x-api-path-slug: teammemberships-membership-delete
      parameters:
      - in: path
        name: _membership
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Membership
  /13f99fq1:
    get:
      summary: Check requestb.in (test purpose)
      description: check an event has been posted
      operationId: 13f99fq1Get
      x-api-path-slug: 13f99fq1-get
      parameters:
      - in: query
        name: inspect
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Check
      - Requestb
      - In
      - (test
      - Purpose)
  /teams/{_team}:
    get:
      summary: Get team details
      description: |-
        Show details for a team.

        https://developer.webex.com/endpoint-teams-teamId-get.html
      operationId: TeamsByTeamGet
      x-api-path-slug: teams-team-get
      parameters:
      - in: path
        name: _team
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
      - Details
    put:
      summary: Update a team
      description: |-
        Update a team.

        https://developer.webex.com/endpoint-teams-teamId-put.html
      operationId: TeamsByTeamPut
      x-api-path-slug: teams-team-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: _team
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
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