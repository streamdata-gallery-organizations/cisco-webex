---
swagger: "2.0"
x-collection-name: Cisco WebEx
x-complete: 1
info:
  title: Webex Teams API
  description: hey-there-thanks-for-checking-out-cisco-webex-for-developers--if-youve-used-cisco-webex-meetings-or-cisco-webex-teams-formerly-cisco-spark-you-know-how-easy-it-is-to-meet-and-collaborate-with-your-team-members-and-customers-the-webex-for-developers-program-opens-up-the-power-behind-the-webex-platform-to-anyone-seeking-to-extend-the-webex-experience-webex-meetings-is-a-powerful-conferencing-solution-that-lets-you-connect-with-anyone-anywhere-in-real-time--by-combining-video-audio-and-content-sharing-webex-meetings-creates-an-effective-conferencing-environment-leading-to-more-productive-meetings-and-increased-productivity--developer-information-for-webex-meetings-will-soon-be-available-on-this-site--in-the-meantime-to-get-started-with-developing-for-webex-meetings-please-see-the-getting-started-guides-over-on-cisco-devnet--keep-reading-for-information-about-webex-teams-webex-teams-makes-staying-in-sync-with-your-teammates-and-customers-easy-conversations-in-webex-teams-take-place-in-virtual-meeting-rooms--some-rooms-live-for-a-few-hours-while-others-become-permanent-fixtures-of-your-teams-workflow-with-titles-like-daily-standup-or-build-status--webex-teams-allows-conversations-to-flow-seamlessly-between-messages-video-calls-and-realtime-whiteboarding-sessions--no-other-solution-brings-together-so-many-facets-of-collaboration-into-a-single-unified-platform-httpsdeveloper-webex-comgettingstarted-html
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
    delete:
      summary: Delete a team
      description: |-
        Delete a team.

        https://developer.webex.com/endpoint-teams-teamId-delete.html
      operationId: TeamsByTeamDelete2
      x-api-path-slug: teams-team-delete
      parameters:
      - in: path
        name: _team
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Team
  /team/memberships:
    get:
      summary: List team memberships
      description: "Lists all team memberships. By default, lists memberships for
        teams to which the authenticated user belongs.\r\n\r\nUse query parameters
        to filter the response.\r\n\r\nUse teamId to list memberships for a team,
        by ID.\r\n\r\nUse either personId or personEmail to filter the results.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-get.html"
      operationId: TeamMembershipsGet
      x-api-path-slug: teammemberships-get
      parameters:
      - in: query
        name: teamId
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Team
      - Memberships
    post:
      summary: Create a team membership
      description: |-
        Add someone to a team by Person ID or email address; optionally making them a moderator.

        https://developer.webex.com/endpoint-teammemberships-post.html
      operationId: TeamMembershipsPost
      x-api-path-slug: teammemberships-post
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
      - Membership
  /people/{_person}:
    get:
      summary: Get person details
      description: "Shows details for a person, by ID.\r\n\r\nSpecify the person ID
        in the personId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-people-personId-get.html"
      operationId: PeopleByPersonGet
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
      - Details
  /webhooks/:
    post:
      summary: Create a webhook (messages/created)
      description: |-
        Creates a webhook for messages/created event.

        Note that you'll need to change the requestb.in URI to your own to see the webhook in action.

        https://developer.webex.com/endpoint-webhooks-post.html
      operationId: WebhooksPost2
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
      - (messages
      - Created)
---