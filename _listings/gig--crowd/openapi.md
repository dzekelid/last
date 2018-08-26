---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/message/new/{withUserId}/{lastMessageId}:
    get:
      summary: Get Message New Withuserid Lastmessageid
      description: Get message new withuserid lastmessageid.
      operationId: getApiV1MessageNewWithuserLastmessage
      x-api-path-slug: apiv1messagenewwithuseridlastmessageid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: lastMessageId
      - in: path
        name: withUserId
      responses:
        200:
          description: OK
      tags:
      - Message
      - New
      - Withuserid
      - Lastmessageid
---