---
name: Cisco WebEx
x-slug: cisco-webex
description: Cisco Webex is the leading enterprise solution for video conferencing
  & web conferencing today. This secure software-based platform for video & audio
  conferencing, group messaging & webinars helps organizations be more productive.Participants
  can join ...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
x-kinRank: "7"
x-alexaRank: "632"
tags: Cisco WebEx
created: "2018-08-29"
modified: "2018-08-29"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/apis.md
specificationVersion: "0.14"
apis:
- name: Webex Teams Admin API - Get Person Details1
  x-api-slug: people-person-get
  description: |-
    Shows details for a person, by ID.
    Specify the person ID in the personId parameter in the URI.

    https://developer.webex.com/endpoint-people-personId-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/people-person-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/people-person-get-openapi.md
- name: Webex Teams Admin API - Update a Person
  x-api-slug: people-person-put
  description: "Update details for a person, by ID.\r\n\r\nSpecify the person ID in
    the personId parameter in the URI. Only an admin can update a person details.\r\n\r\nhttps://developer.webex.com/endpoint-people-personId-put.html\r\n\r\nExample
    Request:\r\n``` json\r\n{\r\n  'emails\" : [ 'johnny.chang@foomail.com', 'jchang@barmail.com'
    ],\r\n  'displayName' : 'John Andersen',\r\n  'firstName' : 'John',\r\n  'lastName'
    : 'Andersen',\r\n  'avatar' : 'https://1efa7a94ed21783e352-c62266528714497a17239ececf39e9e2.ssl.cf1.rackcdn.com/V1~54c844c89e678e5a7b16a306bc2897b9~wx29yGtlTpilEFlYzqPKag==~1600',\r\n
    \ 'orgId' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',\r\n  'roles' :
    [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy',
    'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX'
    ],\r\n  'licenses' : [ 'Y2lzY29zcGFyazovL3VzL1JPT00vOGNkYzQwYzQtZjA5ZS0zY2JhLThjMjYtZGQwZTcwYWRlY2Iy',
    'Y2lzY29zcGFyazovL3VzL1BFT1BMRS9mMDZkNzFhNS0wODMzLTRmYTUtYTcyYS1jYzg5YjI1ZWVlMmX'
    ]\r\n}\r\n```"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/people-person-put-openapi.md
- name: Webex Teams Admin API - Delete a Person
  x-api-slug: people-person-delete
  description: |-
    Remove a person from the system. Only an admin can remove a person.

    Specify the person ID in the personId parameter in the URI.

    https://developer.webex.com/endpoint-people-personId-delete.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/people-person-delete-openapi.md
- name: Webex Teams Admin API - Get roles (to fetch a role id)
  x-api-slug: roles-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/roles-get-openapi.md
- name: Webex Teams Admin API - Get License Details
  x-api-slug: licenses-license-get
  description: "Shows details for a license, by ID.\r\n\r\nSpecify the license ID
    in the licenseId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-licenses-licenseId-get.html\r\n\r\nExample
    Response:\r\n``` json\r\n{\r\n  'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',\r\n
    \ 'displayName' : 'Spark Calling',\r\n  'totalUnits' : '42',\r\n  'consumedUnits'
    : \"8'\r\n}\r\n```"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/licenses-license-get-openapi.md
- name: Webex Teams Admin API - Get Role Details
  x-api-slug: roles-role-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/roles-role-get-openapi.md
- name: Webex Teams Admin API - Get Person Details (me)
  x-api-slug: peopleme-get
  description: |-
    Show the profile for the authenticated user.

    https://developer.webex.com/endpoint-people-me-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/peopleme-get-openapi.md
- name: Webex Teams Admin API - List Events (new messages)
  x-api-slug: events-get
  description: |-
    List events in your organization. Several query parameters are available to filter the response.
    Long result sets will be split into pages.

    https://developer.webex.com/endpoint-events-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/events-get-openapi.md
- name: Webex Teams Admin API - List Licenses
  x-api-slug: licenses-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/licenses-get-openapi.md
- name: Webex Teams Admin API - Get Events Details
  x-api-slug: events-event-get
  description: "Shows details for an event, by event ID.\r\nSpecify the event ID in
    the eventId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-events-eventId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/events-event-get-openapi.md
- name: Webex Teams Admin API - List Organizations
  x-api-slug: organizations-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/organizations-get-openapi.md
- name: Webex Teams Admin API - List people (with exact email)
  x-api-slug: people-get
  description: |-
    List people in your organization.

    https://developer.webex.com/endpoint-people-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/people-get-openapi.md
- name: Webex Teams Admin API - Create a Person (random)
  x-api-slug: people-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/people-post-openapi.md
- name: Webex Teams Admin API - Get Organization Details
  x-api-slug: organizations-organization-get
  description: "Shows details for an organization, by ID.\r\n\r\nSpecify the org ID
    in the orgId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-organizations-orgId-get.html\r\n\r\nExample
    Response:\r\n``` json\r\n{\r\n  'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',\r\n
    \ 'displayName' : 'Acme, Inc.',\r\n  'created' : '2015-10-18T14:26:16+00:00'\r\n}\r\n```"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/organizations-organization-get-openapi.md
- name: Webex Teams API - List webhooks
  x-api-slug: webhooks-get
  description: |-
    Lists all of your webhooks.

    https://developer.webex.com/endpoint-webhooks-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/webhooks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/webhooks-get-openapi.md
- name: Webex Teams API - Create a webhook (all events, all rooms)
  x-api-slug: webhooks-post
  description: |-
    Creates a webhook for messages/created event.

    Note that you'll need to change the requestb.in URI to your own to see the webhook in action.

    https://developer.webex.com/endpoint-webhooks-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/webhooks-post-openapi.md
- name: Webex Teams API - List rooms
  x-api-slug: rooms-get
  description: "List rooms.\r\n\r\nBy default, lists rooms to which the authenticated
    user belongs.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/rooms-get-openapi.md
- name: Webex Teams API - Create a Team room
  x-api-slug: rooms-post
  description: |-
    Creates a room. The authenticated user is automatically added as a member of the room. See the Memberships API to learn how to add more people to the room.

    https://developer.webex.com/endpoint-rooms-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/rooms-post-openapi.md
- name: Webex Teams API - Get membership details
  x-api-slug: memberships-membership-get
  description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
    ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-memberships-membershipId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/memberships-membership-get-openapi.md
- name: Webex Teams API - Update a membership
  x-api-slug: memberships-membership-put
  description: |-
    Updates properties for a membership by ID.

    Specify the membership ID in the membershipId URI parameter.

    https://developer.ciscospark.com/endpoint-memberships-membershipId-put.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/memberships-membership-put-openapi.md
- name: Webex Teams API - Delete membership
  x-api-slug: memberships-membership-delete
  description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in the
    membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-memberships-membershipId-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/memberships-membership-delete-openapi.md
- name: Webex Teams API - Get message details
  x-api-slug: messages-message-get
  description: |-
    Shows details for a message, by message ID.

    Specify the message ID in the messageId parameter in the URI.

    https://developer.webex.com/endpoint-messages-messageId-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/messages-message-get-openapi.md
- name: Webex Teams API - Delete a message
  x-api-slug: messages-message-delete
  description: |-
    Deletes a message, by message ID.

    Specify the message ID in the messageId parameter in the URI.

    https://developer.webex.com/endpoint-messages-messageId-delete.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/messages-message-delete-openapi.md
- name: Webex Teams API - List messages
  x-api-slug: messages-get
  description: "Lists all messages in a room. If present, includes the associated
    media content attachment for each message.\r\n\r\nThe list sorts the messages
    in descending order by creation date.\r\n\r\nhttps://developer.webex.com/endpoint-messages-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/messages-get-openapi.md
- name: Webex Teams API - Create a message (html)
  x-api-slug: messages-post
  description: |-
    HTML is not officially supported by the API, but will work in some cases

    To get more info about message formatting, check https://developer.ciscospark.com/formatting-messages.html

    https://developer.webex.com/endpoint-messages-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/messages-post-openapi.md
- name: Webex Teams API - Get person details (me)
  x-api-slug: peopleme-get
  description: |-
    Show the profile for the authenticated user.

    https://developer.webex.com/endpoint-people-me-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/peopleme-get-openapi.md
- name: Webex Teams API - Get Team room details
  x-api-slug: rooms-room-get
  description: "Shows details for a room, by ID.\r\n\r\nSpecify the room ID in the
    roomId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-roomId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/rooms-room-get-openapi.md
- name: Webex Teams API - Update a room
  x-api-slug: rooms-room-put
  description: "Updates details for a room, by ID.\r\n\r\nSpecify the room ID in the
    roomId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-roomId-put.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/rooms-room-put-openapi.md
- name: Webex Teams API - Delete a Team room
  x-api-slug: rooms-room-delete
  description: "Deletes a room, by ID.\r\n\r\nSpecify the room ID in the roomId parameter
    in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-roomId-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/rooms-room-delete-openapi.md
- name: Webex Teams API - List teams
  x-api-slug: teams-get
  description: |-
    List teams.

    https://developer.webex.com/endpoint-teams-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/teams-get-openapi.md
- name: Webex Teams API - Create a team
  x-api-slug: teams-post
  description: |-
    Create a new team.

    https://developer.webex.com/endpoint-teams-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/teams-post-openapi.md
- name: Webex Teams API - List people (whose name starts with)
  x-api-slug: people-get
  description: |-
    List people in your organization.

    https://developer.webex.com/endpoint-people-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/people-get-openapi.md
- name: Webex Teams API - Get webhook details1
  x-api-slug: webhooks-webhook-get
  description: "Shows details for a webhook, by ID.\r\n\r\nSpecify the webhook ID
    in the webhookId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-webhooks-webhookId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/webhooks-webhook-get-openapi.md
- name: Webex Teams API - Update a webhook
  x-api-slug: webhooks-webhook-put
  description: "Updates a webhook, by ID.\r\n\r\nSpecify the webhook ID in the webhookId
    parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-webhooks-webhookId-put.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/webhooks-webhook-put-openapi.md
- name: Webex Teams API - Delete a webhook1
  x-api-slug: webhooks-webhook-delete
  description: "Deletes a webhook, by ID.\r\n\r\nSpecify the webhook ID in the webhookId
    parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-webhooks-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/webhooks-webhook-delete-openapi.md
- name: Webex Teams API - List memberships (for all rooms)
  x-api-slug: memberships-get
  description: |-
    Lists all room memberships. By default, lists memberships for rooms to which the authenticated user belongs.

    Use query parameters to filter the response.

    Use roomId to list memberships for a room, by ID.

    Use either personId or personEmail to filter the results.

    https://developer.webex.com/endpoint-memberships-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/memberships-get-openapi.md
- name: Webex Teams API - Create a membership
  x-api-slug: memberships-post
  description: |-
    Add someone to a room by Person ID or email address; optionally making them a moderator.

    https://developer.webex.com/endpoint-memberships-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/memberships-post-openapi.md
- name: Webex Teams API - Get team membership details
  x-api-slug: teammemberships-membership-get
  description: "Get details for a membership by ID.\r\n\r\nSpecify the membership
    ID in the membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/teammemberships-membership-get-openapi.md
- name: Webex Teams API - Update a team membership
  x-api-slug: teammemberships-membership-put
  description: |-
    Updates properties for a membership by ID.

    Specify the membership ID in the membershipId URI parameter.

    https://developer.webex.com/endpoint-teammemberships-membershipId-put.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/teammemberships-membership-put-openapi.md
- name: Webex Teams API - Delete a team membership
  x-api-slug: teammemberships-membership-delete
  description: "Deletes a membership by ID.\r\n\r\nSpecify the membership ID in the
    membershipId URI parameter.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-membershipId-delete.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/teammemberships-membership-delete-openapi.md
- name: Webex Teams API - Check requestb.in (test purpose)
  x-api-slug: 13f99fq1-get
  description: check an event has been posted
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/13f99fq1-get-openapi.md
- name: Webex Teams API - Get team details
  x-api-slug: teams-team-get
  description: |-
    Show details for a team.

    https://developer.webex.com/endpoint-teams-teamId-get.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/teams-team-get-openapi.md
- name: Webex Teams API - Update a team
  x-api-slug: teams-team-put
  description: |-
    Update a team.

    https://developer.webex.com/endpoint-teams-teamId-put.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/teams-team-put-openapi.md
- name: Webex Teams API - Delete a team
  x-api-slug: teams-team-delete
  description: |-
    Delete a team.

    https://developer.webex.com/endpoint-teams-teamId-delete.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/teams-team-delete-openapi.md
- name: Webex Teams API - List team memberships
  x-api-slug: teammemberships-get
  description: "Lists all team memberships. By default, lists memberships for teams
    to which the authenticated user belongs.\r\n\r\nUse query parameters to filter
    the response.\r\n\r\nUse teamId to list memberships for a team, by ID.\r\n\r\nUse
    either personId or personEmail to filter the results.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/teammemberships-get-openapi.md
- name: Webex Teams API - Create a team membership
  x-api-slug: teammemberships-post
  description: |-
    Add someone to a team by Person ID or email address; optionally making them a moderator.

    https://developer.webex.com/endpoint-teammemberships-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/teammemberships-post-openapi.md
- name: Webex Teams API - Get person details
  x-api-slug: people-person-get
  description: "Shows details for a person, by ID.\r\n\r\nSpecify the person ID in
    the personId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-people-personId-get.html"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/people-person-get-openapi.md
- name: Webex Teams API - Create a webhook (messages/created)
  x-api-slug: webhooks-post
  description: |-
    Creates a webhook for messages/created event.

    Note that you'll need to change the requestb.in URI to your own to see the webhook in action.

    https://developer.webex.com/endpoint-webhooks-post.html
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/730-cisco-webex.jpg
  humanURL: https://webex.com
  baseURL: https://api.ciscospark.com//v1
  tags: Enterprise, Office, Collaboration, Video Conferencing, SaaS, Technology, Telecommunications,
    API Provider, Profiles, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/cisco-webex/master/_listings/cisco-webex/webhooks-post-openapi.md
x-common:
- type: x-postman-collection
  url: https://app.getpostman.com/run-collection/1f5e101d8290a5303c90
- type: x-api-gallery
  url: http://cisco.unity.connection.messaging.interface.api.gallery.streamdata.io
- type: x-api-stack
  url: http://cisco.webex.stack.network
- type: x-blog
  url: http://blogs.webex.com/
- type: x-blog-rss
  url: http://blogs.webex.com/webex_interactions/index.rdf
- type: x-crunchbase
  url: https://crunchbase.com/organization/webex-communications
- type: x-crunchbase
  url: http://www.crunchbase.com/company/webex
- type: x-postman-collection
  url: https://app.getpostman.com/run-collection/0aa22af74405f82086d4
- type: x-twitter
  url: https://twitter.com/webex
- type: x-developer
  url: https://developer.webex.com/
- type: x-website
  url: https://webex.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---