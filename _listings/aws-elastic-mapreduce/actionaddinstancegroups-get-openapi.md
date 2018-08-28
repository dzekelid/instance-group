---
swagger: "2.0"
x-collection-name: AWS Elastic MapReduce
x-complete: 0
info:
  title: AWS Elastic MapReduce API Add Instance Groups
  version: 1.0.0
  description: Adds one or more instance groups to a running cluster.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddInstanceGroups:
    get:
      summary: Add Instance Groups
      description: Adds one or more instance groups to a running cluster.
      operationId: addInstanceGroups
      x-api-path-slug: actionaddinstancegroups-get
      parameters:
      - in: query
        name: InstanceGroups
        description: Instance groups to add
        type: string
      - in: query
        name: JobFlowId
        description: Job flow in which to add the instance groups
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Groups
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