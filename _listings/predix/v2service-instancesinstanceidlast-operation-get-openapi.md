---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Event Audit Trail Get Service Instances Last Operation
  description: Get service instances last operation.
  version: 1.0.0
host: event-audit-trail.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/usage:
    get:
      summary: Get last usage
      description: get last usage by zoneid
      operationId: get-last-usage-by-zoneid
      x-api-path-slug: reportsusage-get
      parameters:
      - in: header
        name: Authorization
        description: Basic *token
      - in: header
        name: predix-zone-id
        description: Cloud Foundry service instance id
      responses:
        200:
          description: Successful response
      tags:
      - Last
      - Usage
  /v2/service_instances/{instanceId}/last_operation:
    get:
      summary: Get Service Instances Last Operation
      description: Get service instances last operation.
      operationId: getV2ServiceInstancesInstanceLastOperation
      x-api-path-slug: v2service-instancesinstanceidlast-operation-get
      parameters:
      - in: path
        name: instanceId
        description: instanceId
      responses:
        200:
          description: Successful response
      tags:
      - Service
      - Instances
      - Last
      - Operation
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