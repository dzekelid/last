---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 1
info:
  title: AWS Identity and Access Management API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetAccessKeyLastUsed:
    get:
      summary: Get Access Key Last Used
      description: Retrieves information about when the specified access key was last
        used.
      operationId: getAccessKeyLastUsed
      x-api-path-slug: actiongetaccesskeylastused-get
      parameters:
      - in: query
        name: AccessKeyId
        description: The identifier of an access key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Access Keys
---