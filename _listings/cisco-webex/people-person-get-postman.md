{
  "info": {
    "name": "Webex Teams Admin API Get Person Details1",
    "_postman_id": "dfc41bd3-7a97-42b3-baa6-2fb4dab3d91b",
    "description": "Shows details for a person, by ID.\nSpecify the person ID in the personId parameter in the URI.\n\nhttps://developer.webex.com/endpoint-people-personId-get.html",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Video Conferencing",
      "item": [
        {
          "id": "1f61016a-64ea-480f-863a-73bec77513e6",
          "name": "PeopleByPersonGet2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.ciscospark.com",
              "path": [
                "v1",
                "people/:_person"
              ],
              "variable": [
                {
                  "id": "_person",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows details for a person, by ID.\nSpecify the person ID in the personId parameter in the URI.\n\nhttps://developer.webex.com/endpoint-people-personId-get.html"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2b226bd-44ce-48e8-b082-0706c5d462f2"
            }
          ]
        }
      ]
    }
  ]
}