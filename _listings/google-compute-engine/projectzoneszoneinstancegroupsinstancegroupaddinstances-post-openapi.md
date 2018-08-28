---
swagger: "2.0"
x-collection-name: Google Compute Engine
x-complete: 0
info:
  title: Google Compute Engine API Add Instance to Zone Instance Group
  description: Adds a list of instances to the specified instance group. All of the
    instances in the instance group must be in the same network/subnetwork. Read  Adding
    instances for more information.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /compute/v1/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/aggregated/instanceGroupManagers:
    get:
      summary: Get Instance Group Managers
      description: Retrieves the list of managed instance groups and groups them by
        zone.
      operationId: compute.instanceGroupManagers.aggregatedList
      x-api-path-slug: projectaggregatedinstancegroupmanagers-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Instance Group
  /{project}/aggregated/instanceGroups:
    get:
      summary: Get Instance Groups
      description: Retrieves the list of instance groups and sorts them by zone.
      operationId: compute.instanceGroups.aggregatedList
      x-api-path-slug: projectaggregatedinstancegroups-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Instance Group
      - Aggregation
  /{project}/regions/{region}/instanceGroupManagers:
    get:
      summary: Get Instance Group Managers
      description: Retrieves the list of managed instance groups that are contained
        within the specified region.
      operationId: compute.regionInstanceGroupManagers.list
      x-api-path-slug: projectregionsregioninstancegroupmanagers-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance Group
    post:
      summary: Create Instance Group Manager
      description: Creates a managed instance group using the information that you
        specify in the request. After the group is created, it schedules an action
        to create instances in the group using the specified instance template. This
        operation is marked as DONE when the group is created even if the instances
        in the group have not yet been created. You must separately verify the status
        of the individual instances with the listmanagedinstances method.
      operationId: compute.regionInstanceGroupManagers.insert
      x-api-path-slug: projectregionsregioninstancegroupmanagers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance Group
  /{project}/regions/{region}/instanceGroupManagers/{instanceGroupManager}:
    delete:
      summary: Delete Instance Group Manager
      description: Deletes the specified managed instance group and all of the instances
        in that group.
      operationId: compute.regionInstanceGroupManagers.delete
      x-api-path-slug: projectregionsregioninstancegroupmanagersinstancegroupmanager-delete
      parameters:
      - in: path
        name: instanceGroupManager
        description: Name of the managed instance group to delete
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance Group
    get:
      summary: Get Instance Group Manager
      description: Returns all of the details about the specified managed instance
        group.
      operationId: compute.regionInstanceGroupManagers.get
      x-api-path-slug: projectregionsregioninstancegroupmanagersinstancegroupmanager-get
      parameters:
      - in: path
        name: instanceGroupManager
        description: Name of the managed instance group to return
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance Group
  /{project}/regions/{region}/instanceGroups:
    get:
      summary: Get Instance Groups
      description: Retrieves the list of instance group resources contained within
        the specified region.
      operationId: compute.regionInstanceGroups.list
      x-api-path-slug: projectregionsregioninstancegroups-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance Group
  /{project}/regions/{region}/instanceGroups/{instanceGroup}:
    get:
      summary: Get Instance Group
      description: Returns the specified instance group resource.
      operationId: compute.regionInstanceGroups.get
      x-api-path-slug: projectregionsregioninstancegroupsinstancegroup-get
      parameters:
      - in: path
        name: instanceGroup
        description: Name of the instance group resource to return
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance Group
  /{project}/regions/{region}/instanceGroups/{instanceGroup}/setNamedPorts:
    post:
      summary: Set Named Portal
      description: Sets the named ports for the specified regional instance group.
      operationId: compute.regionInstanceGroups.setNamedPorts
      x-api-path-slug: projectregionsregioninstancegroupsinstancegroupsetnamedports-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instanceGroup
        description: The name of the regional instance group where the named ports
          are updated
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: region
        description: Name of the region scoping this request
      responses:
        200:
          description: OK
      tags:
      - Instance Group
  /{project}/zones/{zone}/instanceGroups:
    get:
      summary: Get Zone Instance Groups
      description: Retrieves the list of instance groups that are located in the specified
        project and zone.
      operationId: compute.instanceGroups.list
      x-api-path-slug: projectzoneszoneinstancegroups-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone where the instance group is located
      responses:
        200:
          description: OK
      tags:
      - Instance Group
    post:
      summary: Create Zone Instance Group
      description: Creates an instance group in the specified project using the parameters
        that are included in the request.
      operationId: compute.instanceGroups.insert
      x-api-path-slug: projectzoneszoneinstancegroups-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone where you want to create the instance group
      responses:
        200:
          description: OK
      tags:
      - Instance Group
  /{project}/zones/{zone}/instanceGroups/{instanceGroup}:
    delete:
      summary: Delete Zone Instance Group
      description: Deletes the specified instance group. The instances in the group
        are not deleted. Note that instance group must not belong to a backend service.
        Read  Deleting an instance group for more information.
      operationId: compute.instanceGroups.delete
      x-api-path-slug: projectzoneszoneinstancegroupsinstancegroup-delete
      parameters:
      - in: path
        name: instanceGroup
        description: The name of the instance group to delete
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone where the instance group is located
      responses:
        200:
          description: OK
      tags:
      - Instance Group
    get:
      summary: Get Zone Instance Group
      description: Returns the specified instance group. Get a list of available instance
        groups by making a list() request.
      operationId: compute.instanceGroups.get
      x-api-path-slug: projectzoneszoneinstancegroupsinstancegroup-get
      parameters:
      - in: path
        name: instanceGroup
        description: The name of the instance group
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone where the instance group is located
      responses:
        200:
          description: OK
      tags:
      - Instance Group
  /{project}/zones/{zone}/instanceGroups/{instanceGroup}/addInstances:
    post:
      summary: Add Instance to Zone Instance Group
      description: Adds a list of instances to the specified instance group. All of
        the instances in the instance group must be in the same network/subnetwork.
        Read  Adding instances for more information.
      operationId: compute.instanceGroups.addInstances
      x-api-path-slug: projectzoneszoneinstancegroupsinstancegroupaddinstances-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: instanceGroup
        description: The name of the instance group where you are adding instances
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: zone
        description: The name of the zone where the instance group is located
      responses:
        200:
          description: OK
      tags:
      - Instance Group
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