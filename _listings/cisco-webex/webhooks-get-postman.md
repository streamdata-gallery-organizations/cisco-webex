{
  "info": {
    "name": "WebEx Teams API List webhooks",
    "_postman_id": "682c072c-f708-4ee2-8d04-b0e34ec9a749",
    "description": "Lists all of your webhooks.\n\nhttps://developer.webex.com/endpoint-webhooks-get.html",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Video Conferencing",
      "item": [
        {
          "id": "e5432e98-1be8-498c-9d78-228610291e12",
          "name": "WebhooksGet",
          "request": {
            "url": "http://api.ciscospark.com/v1/webhooks",
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
            "description": "Lists all of your webhooks.\n\nhttps://developer.webex.com/endpoint-webhooks-get.html"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2bfc0b48-5fa4-4d63-a362-cdc22705715e"
            }
          ]
        }
      ]
    }
  ]
}