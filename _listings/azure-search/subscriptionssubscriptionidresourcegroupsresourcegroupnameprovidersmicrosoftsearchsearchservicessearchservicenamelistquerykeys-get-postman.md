{
  "info": {
    "name": "Azure Search API Query Keys List By Search Service",
    "_postman_id": "882ed3a6-bd6e-4287-80b6-2eea931c8e8c",
    "description": "Returns the list of query API keys for the given Azure Search service.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "query keys",
      "item": [
        {
          "id": "f7ec8db3-7f3d-4f3f-a00b-1e61263d0211",
          "name": "QueryKeys_ListBySearchService",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Search/searchServices/:searchServiceName/listQueryKeys"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "searchServiceName",
                  "value": "searchServiceName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of query API keys for the given Azure Search service"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d40a961-193a-40d7-a009-2f4f9651f018"
            }
          ]
        }
      ]
    }
  ]
}