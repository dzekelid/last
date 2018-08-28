{
  "info": {
    "name": "Steem get_replies_by_last_update",
    "_postman_id": "f125dd7f-b21b-45fd-aff3-70f92e8b4dac",
    "description": "get_replies_by_last_update",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "2157eddf-ae67-4a30-a562-28b068cdfb45",
          "name": "get-replies-by-last-update",
          "request": {
            "url": "http://api.steemjs.com/get_replies_by_last_update?limit=%7B%7D&startAuthor=%7B%7D&startPermlink=%7B%7D",
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
            "description": "get_replies_by_last_update"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f201062-016a-4a2b-b9c3-9d672c091f0a"
            }
          ]
        }
      ]
    }
  ]
}