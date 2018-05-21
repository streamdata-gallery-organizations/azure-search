---
swagger: "2.0"
x-collection-name: Azure Search
x-complete: 1
info:
  title: SearchManagementClient
  description: client-that-can-be-used-to-manage-azure-search-services-and-api-keys
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}/listAdminKeys
  : post:
      summary: Admin Keys Get
      description: Gets the primary and secondary admin API keys for the specified
        Azure Search service.
      operationId: AdminKeys_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicenamelistadminkeys-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Admin Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}/regenerateAdminKey/{keyKind}
  : post:
      summary: Admin Keys Regenerate
      description: Regenerates either the primary or secondary admin API key. You
        can only regenerate one key at a time.
      operationId: AdminKeys_Regenerate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicenameregenerateadminkeykeykind-post
      parameters:
      - in: path
        name: keyKind
        description: Specifies which key to regenerate
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Admin Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}/createQueryKey/{name}
  : post:
      summary: Query Keys Create
      description: Generates a new query key for the specified Search service. You
        can create up to 50 query keys per service.
      operationId: QueryKeys_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicenamecreatequerykeyname-post
      parameters:
      - in: path
        name: name
        description: The name of the new query API key
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Query Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}/listQueryKeys
  : get:
      summary: Query Keys List By Search Service
      description: Returns the list of query API keys for the given Azure Search service.
      operationId: QueryKeys_ListBySearchService
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicenamelistquerykeys-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Query Keys
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}/deleteQueryKey/{key}
  : delete:
      summary: Query Keys Delete
      description: Deletes the specified query key. Unlike admin keys, query keys
        are not regenerated. The process for regenerating a query key is to delete
        and then recreate it.
      operationId: QueryKeys_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicenamedeletequerykeykey-delete
      parameters:
      - in: path
        name: key
        description: The query key to be deleted
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Query Keys
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}:
    put:
      summary: Services Create Or Update
      description: Creates or updates a Search service in the given resource group.
        If the Search service already exists, all properties will be updated with
        the given values.
      operationId: Services_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicename-put
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
      - Services
    get:
      summary: Services Get
      description: Gets the Search service with the given name in the given resource
        group.
      operationId: Services_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicename-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Services
    delete:
      summary: Services Delete
      description: Deletes a Search service in the given resource group, along with
        its associated resources.
      operationId: Services_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicename-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Services
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices:
    get:
      summary: Services List By Resource Group
      description: Gets a list of all Search services in the given resource group.
      operationId: Services_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservices-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Services Resource Group
  /subscriptions/{subscriptionId}/providers/Microsoft.Search/checkNameAvailability:
    post:
      summary: Services Check Name Availability
      description: Checks whether or not the given Search service name is available
        for use. Search service names must be globally unique since they are part
        of the service URI (https://<name>.search.windows.net).
      operationId: Services_CheckNameAvailability
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftsearchchecknameavailability-post
      parameters:
      - in: body
        name: checkNameAvailabilityInput
        description: The resource name and type to check
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Services Name Availability
---