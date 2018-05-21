---
name: Azure Search
x-slug: azure-search
description: Azure Search is a fully-managed service for adding sophisticated search
  capabilities to web and mobile applications without the typical complexities of
  full-text search.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
x-kinRank: "10"
x-alexaRank: ""
tags: Azure Search
created: "2018-05-21"
modified: "2018-05-21"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Search API Admin Keys Get
  x-api-slug: azure-search-api
  description: Gets the primary and secondary admin API keys for the specified Azure
    Search service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}/listAdminKeys
  tags: Admin Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicenamelistadminkeys-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicenamelistadminkeys-post-openapi.md
- name: Azure Search API Admin Keys Regenerate
  x-api-slug: azure-search-api
  description: Regenerates either the primary or secondary admin API key. You can
    only regenerate one key at a time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}/regenerateAdminKey/{keyKind}
  tags: Admin Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicenameregenerateadminkeykeykind-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicenameregenerateadminkeykeykind-post-openapi.md
- name: Azure Search API Query Keys Create
  x-api-slug: azure-search-api
  description: Generates a new query key for the specified Search service. You can
    create up to 50 query keys per service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}/createQueryKey/{name}
  tags: Query Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicenamecreatequerykeyname-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicenamecreatequerykeyname-post-openapi.md
- name: Azure Search API Query Keys List By Search Service
  x-api-slug: azure-search-api
  description: Returns the list of query API keys for the given Azure Search service.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}/listQueryKeys
  tags: Query Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicenamelistquerykeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicenamelistquerykeys-get-openapi.md
- name: Azure Search API Query Keys Delete
  x-api-slug: azure-search-api
  description: Deletes the specified query key. Unlike admin keys, query keys are
    not regenerated. The process for regenerating a query key is to delete and then
    recreate it.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}/deleteQueryKey/{key}
  tags: Query Keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicenamedeletequerykeykey-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicenamedeletequerykeykey-delete-openapi.md
- name: Azure Search API Services Create Or Update
  x-api-slug: azure-search-api
  description: Creates or updates a Search service in the given resource group. If
    the Search service already exists, all properties will be updated with the given
    values.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}
  tags: Services
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicename-put-openapi.md
- name: Azure Search API Services Get
  x-api-slug: azure-search-api
  description: Gets the Search service with the given name in the given resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}
  tags: Services
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicename-get-openapi.md
- name: Azure Search API Services Delete
  x-api-slug: azure-search-api
  description: Deletes a Search service in the given resource group, along with its
    associated resources.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices/{searchServiceName}
  tags: Services
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicename-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservicessearchservicename-delete-openapi.md
- name: Azure Search API Services List By Resource Group
  x-api-slug: azure-search-api
  description: Gets a list of all Search services in the given resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Search/searchServices
  tags: Services Resource Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservices-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsearchsearchservices-get-openapi.md
- name: Azure Search API Services Check Name Availability
  x-api-slug: azure-search-api
  description: Checks whether or not the given Search service name is available for
    use. Search service names must be globally unique since they are part of the service
    URI (https://<name>.search.windows.net).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Search/checkNameAvailability
  tags: Services Name Availability
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/subscriptionssubscriptionidprovidersmicrosoftsearchchecknameavailability-post-openapi.md
- name: Azure Search API
  x-api-slug: azure-search-api
  description: Azure Search is a fully-managed service for adding sophisticated search
    capabilities to web and mobile applications without the typical complexities of
    full-text search.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-search.png
  humanURL: https://azure.microsoft.com/en-us/services/search/
  baseURL: ://management.azure.com//
  tags: Azure Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-search/master/_listings/azure-search/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/search/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/search/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/search/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/search/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---