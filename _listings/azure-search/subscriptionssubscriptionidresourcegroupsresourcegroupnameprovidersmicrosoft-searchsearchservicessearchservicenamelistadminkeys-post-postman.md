{
  "info": {
    "name": "Azure Search API Admin Keys Get",
    "_postman_id": "d9e8783c-7727-4e6d-8949-25a5cffb1e1e",
    "description": "Gets the primary and secondary admin API keys for the specified Azure Search service.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "admin keys",
      "item": [
        {
          "id": "3d682e64-6b07-4cca-9972-7bc17ed832b6",
          "name": "AdminKeys_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Search/searchServices/:searchServiceName/listAdminKeys"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the primary and secondary admin API keys for the specified Azure Search service"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3c029eb-8824-42b4-8858-c2206c7c2cf9"
            }
          ]
        }
      ]
    }
  ]
}