{
  "info": {
    "name": "Azure Search API Services Get",
    "_postman_id": "105cb74e-8428-4af7-9954-201fd8dc97c4",
    "description": "Gets the Search service with the given name in the given resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "services",
      "item": [
        {
          "id": "d705b758-f937-4228-a9cb-8c4bc1a09e1b",
          "name": "Services_Get",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the Search service with the given name in the given resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d0f997a-513b-46aa-bc46-617b3e01f16a"
            }
          ]
        }
      ]
    }
  ]
}