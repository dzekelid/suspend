---
swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 0
info:
  title: AWS Auto Scaling API Suspend Processes
  version: 1.0.0
  description: Suspends the specified Auto Scaling processes, or all processes, for
    the specified Auto Scaling group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SuspendProcesses:
    get:
      summary: Suspend Processes
      description: Suspends the specified Auto Scaling processes, or all processes,
        for the specified Auto Scaling group.
      operationId: suspendProcesses
      x-api-path-slug: actionsuspendprocesses-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name or Amazon Resource Name (ARN) of the Auto Scaling group
        type: string
      - in: query
        name: ScalingProcesses.member.N
        description: One or more of the following processes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Processes
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