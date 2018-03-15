---
swagger: "2.0"
info:
  title: SearchManagementClient
  description: Client that can be used to manage Azure Search services and API keys.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}:
    put:
      summary: Services Create Or Update
      description: Creates or updates a Search service in the given resource group
      operationId: Services_CreateOrUpdate
      parameters:
      - in: query
        name: No Name
      - in: path
        name: searchServiceName
        description: The name of the Azure Search service to create or update
      - in: body
        name: service
        description: The definition of the Search service to create or update
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - services
definitions:
  CheckNameAvailabilityInput:
    properties:
      name:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  CheckNameAvailabilityOutput:
    properties:
      nameAvailable:
        description: This is a default description.
        type: post
      reason:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  AdminKeyResult:
    properties:
      primaryKey:
        description: This is a default description.
        type: post
      secondaryKey:
        description: This is a default description.
        type: post
  QueryKey:
    properties:
      name:
        description: This is a default description.
        type: post
      key:
        description: This is a default description.
        type: post
  ListQueryKeysResult:
    properties:
      value:
        description: This is a default description.
        type: post
  Sku:
    properties:
      name:
        description: This is a default description.
        type: post
  SearchService:
    properties: []
  SearchServiceProperties:
    properties:
      replicaCount:
        description: This is a default description.
        type: post
      partitionCount:
        description: This is a default description.
        type: post
      hostingMode:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
      statusDetails:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
  SearchServiceListResult:
    properties:
      value:
        description: This is a default description.
        type: post
  Resource:
    properties:
      id:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
      tags:
        description: This is a default description.
        type: post
  CloudError:
    properties: []
  CloudErrorBody:
    properties:
      code:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
      target:
        description: This is a default description.
        type: post
      details:
        description: This is a default description.
        type: post
x-collection-name: Azure Search
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