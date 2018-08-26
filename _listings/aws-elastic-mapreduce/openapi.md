---
swagger: "2.0"
x-collection-name: AWS Elastic MapReduce
x-complete: 1
info:
  title: AWS Elastic MapReduce API
  version: 1.0.0
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
  /?Action=ListInstanceGroups:
    get:
      summary: List Instance Groups
      description: Provides all available details about the instance groups in a cluster.
      operationId: listInstanceGroups
      x-api-path-slug: actionlistinstancegroups-get
      parameters:
      - in: query
        name: ClusterId
        description: The identifier of the cluster for which to list the instance
          groups
        type: string
      - in: query
        name: Marker
        description: The pagination token that indicates the next set of results to
          retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Groups
  /?Action=ModifyInstanceGroups:
    get:
      summary: Modify Instance Groups
      description: ModifyInstanceGroups modifies the number of nodes and configuration
        settings of an instance group.
      operationId: modifyInstanceGroups
      x-api-path-slug: actionmodifyinstancegroups-get
      parameters:
      - in: query
        name: ClusterId
        description: The ID of the cluster to which the instance group belongs
        type: string
      - in: query
        name: InstanceGroups
        description: Instance groups to change
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instance Groups
---