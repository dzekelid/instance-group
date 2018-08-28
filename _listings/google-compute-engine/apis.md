---
name: Google Compute Engine
x-slug: google-compute-engine
description: Google Compute Engine delivers virtual machines running in Googles innovative
  data centers and worldwide fiber network. Compute Engines tooling and workflow support
  enable scaling from single instances to global, load-balanced cloud computing.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Instance Group
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/apis.md
specificationVersion: "0.14"
apis:
- name: Compute Engine - Get Instance Group Managers
  x-api-slug: projectaggregatedinstancegroupmanagers-get
  description: Retrieves the list of managed instance groups and groups them by zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectaggregatedinstancegroupmanagers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectaggregatedinstancegroupmanagers-get-openapi.md
- name: Compute Engine - Get Instance Groups
  x-api-slug: projectaggregatedinstancegroups-get
  description: Retrieves the list of instance groups and sorts them by zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectaggregatedinstancegroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectaggregatedinstancegroups-get-openapi.md
- name: Compute Engine - Get Instance Group Managers
  x-api-slug: projectregionsregioninstancegroupmanagers-get
  description: Retrieves the list of managed instance groups that are contained within
    the specified region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagers-get-openapi.md
- name: Compute Engine - Create Instance Group Manager
  x-api-slug: projectregionsregioninstancegroupmanagers-post
  description: Creates a managed instance group using the information that you specify
    in the request. After the group is created, it schedules an action to create instances
    in the group using the specified instance template. This operation is marked as
    DONE when the group is created even if the instances in the group have not yet
    been created. You must separately verify the status of the individual instances
    with the listmanagedinstances method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagers-post-openapi.md
- name: Compute Engine - Delete Instance Group Manager
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanager-delete
  description: Deletes the specified managed instance group and all of the instances
    in that group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanager-delete-openapi.md
- name: Compute Engine - Get Instance Group Manager
  x-api-slug: projectregionsregioninstancegroupmanagersinstancegroupmanager-get
  description: Returns all of the details about the specified managed instance group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectregionsregioninstancegroupmanagersinstancegroupmanager-get-openapi.md
- name: Compute Engine - Get Instance Groups
  x-api-slug: projectregionsregioninstancegroups-get
  description: Retrieves the list of instance group resources contained within the
    specified region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectregionsregioninstancegroups-get-openapi.md
- name: Compute Engine - Get Instance Group
  x-api-slug: projectregionsregioninstancegroupsinstancegroup-get
  description: Returns the specified instance group resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectregionsregioninstancegroupsinstancegroup-get-openapi.md
- name: Compute Engine - Set Named Portal
  x-api-slug: projectregionsregioninstancegroupsinstancegroupsetnamedports-post
  description: Sets the named ports for the specified regional instance group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectregionsregioninstancegroupsinstancegroupsetnamedports-post-openapi.md
- name: Compute Engine - Get Zone Instance Groups
  x-api-slug: projectzoneszoneinstancegroups-get
  description: Retrieves the list of instance groups that are located in the specified
    project and zone.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectzoneszoneinstancegroups-get-openapi.md
- name: Compute Engine - Create Zone Instance Group
  x-api-slug: projectzoneszoneinstancegroups-post
  description: Creates an instance group in the specified project using the parameters
    that are included in the request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectzoneszoneinstancegroups-post-openapi.md
- name: Compute Engine - Delete Zone Instance Group
  x-api-slug: projectzoneszoneinstancegroupsinstancegroup-delete
  description: Deletes the specified instance group. The instances in the group are
    not deleted. Note that instance group must not belong to a backend service. Read  Deleting
    an instance group for more information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectzoneszoneinstancegroupsinstancegroup-delete-openapi.md
- name: Compute Engine - Get Zone Instance Group
  x-api-slug: projectzoneszoneinstancegroupsinstancegroup-get
  description: Returns the specified instance group. Get a list of available instance
    groups by making a list() request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectzoneszoneinstancegroupsinstancegroup-get-openapi.md
- name: Compute Engine - Add Instance to Zone Instance Group
  x-api-slug: projectzoneszoneinstancegroupsinstancegroupaddinstances-post
  description: Adds a list of instances to the specified instance group. All of the
    instances in the instance group must be in the same network/subnetwork. Read  Adding
    instances for more information.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectzoneszoneinstancegroupsinstancegroupaddinstances-post-openapi.md
- name: Compute Engine - Get Instance in Zone Instance Group
  x-api-slug: projectzoneszoneinstancegroupsinstancegrouplistinstances-post
  description: Lists the instances in the specified instance group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectzoneszoneinstancegroupsinstancegrouplistinstances-post-openapi.md
- name: Compute Engine - Remove Instance in Zone Instance Group
  x-api-slug: projectzoneszoneinstancegroupsinstancegroupremoveinstances-post
  description: Removes one or more instances from the specified instance group, but
    does not delete those instances.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectzoneszoneinstancegroupsinstancegroupremoveinstances-post-openapi.md
- name: Compute Engine - Set Named Ports for Zone Instance Group
  x-api-slug: projectzoneszoneinstancegroupsinstancegroupsetnamedports-post
  description: Sets the named ports for the specified instance group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google_Compute_Engine_logo.png
  humanURL: https://cloud.google.com/compute/
  baseURL: ://www.googleapis.com//compute/v1/projects
  tags: Compute, Cloud, Google APIs, Stack Network, API Service Provider, API Provider,
    Deployments, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/instance-group/master/_listings/google-compute-engine/projectzoneszoneinstancegroupsinstancegroupsetnamedports-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.cloud.vision.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.compute.engine.stack.network
- type: x-code
  url: https://cloud.google.com/compute/docs/api/libraries
- type: x-documentation
  url: https://cloud.google.com/compute/docs/reference/latest/
- type: x-guides
  url: https://cloud.google.com/compute/docs/api/how-tos/how-tos
- type: x-rate-limits
  url: https://cloud.google.com/compute/docs/api-rate-limits
- type: x-sla
  url: https://cloud.google.com/compute/sla
- type: x-website
  url: https://cloud.google.com/compute/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---