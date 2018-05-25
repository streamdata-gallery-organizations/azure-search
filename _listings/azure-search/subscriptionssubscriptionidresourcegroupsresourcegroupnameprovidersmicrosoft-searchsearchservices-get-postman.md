{
  "info": {
    "name": "Azure Search API Services List By Resource Group",
    "_postman_id": "fbd4c133-c01c-4f07-9e27-7a687001af3b",
    "description": "Gets a list of all Search services in the given resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "services resource group",
      "item": [
        {
          "id": "f6e6e4ba-673a-4f5b-9b65-172811e81ed6",
          "name": "Services_ListByResourceGroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Search/searchServices"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of all Search services in the given resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4976cad2-aa14-4c76-949a-f5d6fcca92cf"
            }
          ]
        }
      ]
    }
  ]
}