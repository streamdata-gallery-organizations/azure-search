{
  "info": {
    "name": "Azure Search API Services Delete",
    "_postman_id": "3658d2c7-bf37-4617-891d-d86ec384365f",
    "description": "Deletes a Search service in the given resource group, along with its associated resources.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "services",
      "item": [
        {
          "id": "09bbc4c3-630a-43e5-bcdf-26de7b025f3f",
          "name": "Services_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Search/searchServices/:searchServiceName"
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a Search service in the given resource group, along with its associated resources"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "def77843-63e6-4dac-8783-63719997c72a"
            }
          ]
        }
      ]
    }
  ]
}