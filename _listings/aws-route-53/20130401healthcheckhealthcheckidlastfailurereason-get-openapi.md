---
swagger: "2.0"
x-collection-name: AWS Route 53
x-complete: 0
info:
  title: AWS Route 53 API Get Health Check Last Failure Reason
  version: 1.0.0
  description: If you want to learn why a health check is currently failing or why
    it failed mostrecently (if at all), you can get the failure reason for the most
    recent failure. Send aGET request to the /Amazon Route 53 APIversion/healthcheck/health
    checkID/lastfailurereason resource.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2013-04-01/healthcheck/HealthCheckId/lastfailurereason:
    get:
      summary: Get Health Check Last Failure Reason
      description: If you want to learn why a health check is currently failing or
        why it failed mostrecently (if at all), you can get the failure reason for
        the most recent failure. Send aGET request to the /Amazon Route 53 APIversion/healthcheck/health
        checkID/lastfailurereason resource.
      operationId: gethealthchecklastfailurereason
      x-api-path-slug: 20130401healthcheckhealthcheckidlastfailurereason-get
      parameters:
      - in: path
        name: HealthCheckId
        description: The ID for the health check for which you want the last failure
          reason
        type: string
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Health
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