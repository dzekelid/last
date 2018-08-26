---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/ClientFirstNameLastName:
    post:
      summary: Add API Clientfirstnamelastname
      description: Add api clientfirstnamelastname.
      operationId: ApiClientFirstNameLastNamePost
      x-api-path-slug: apiclientfirstnamelastname-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Clientfirstnamelastname
  /api/LastBaseAssets:
    get:
      summary: Get API Lastbaseassets
      description: Get api lastbaseassets.
      operationId: ApiLastBaseAssetsGet
      x-api-path-slug: apilastbaseassets-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: "n"
      responses:
        200:
          description: OK
      tags:
      - Lastbaseassets
---