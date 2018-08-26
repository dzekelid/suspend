---
swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 1
info:
  title: AWS Auto Scaling API
  version: 1.0.0
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
---