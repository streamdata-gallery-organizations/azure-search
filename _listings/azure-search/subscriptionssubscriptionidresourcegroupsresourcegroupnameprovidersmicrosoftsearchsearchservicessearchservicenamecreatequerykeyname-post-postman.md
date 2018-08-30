{
  "info": {
    "name": "Azure Search API Query Keys Create",
    "_postman_id": "f4c19fe6-7402-4411-b75d-fcf1072f19e1",
    "description": "Generates a new query key for the specified Search service. You can create up to 50 query keys per service.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "query keys",
      "item": [
        {
          "id": "f05db28a-0940-41fd-92d7-d1de465ee6d5",
          "name": "QueryKeys_Create",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Search/searchServices/:searchServiceName/createQueryKey/:name"
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
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Generates a new query key for the specified Search service"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3cefd050-dbf7-4739-a3f3-2960b7894034"
            }
          ]
        }
      ]
    }
  ]
}