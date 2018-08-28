---
swagger: "2.0"
x-collection-name: RingCentral
x-complete: 0
info:
  title: RingCentral Suspend Webhook
  description: |-
    Suspends webhooks by ID.
    Usage Plan Group
    Medium
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/glip/webhooks/{webhookId}/suspend:
    post:
      summary: Suspend Webhook
      description: |-
        Suspends webhooks by ID.
        Usage Plan Group
        Medium
      operationId: suspendGlipWebhook
      x-api-path-slug: restapiv1-0glipwebhookswebhookidsuspend-post
      parameters:
      - in: path
        name: webhookId
        description: Internal identifier of a webhook
      responses:
        200:
          description: OK
      tags:
      - Suspend
      - Webhook
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