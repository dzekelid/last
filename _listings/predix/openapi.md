swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
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