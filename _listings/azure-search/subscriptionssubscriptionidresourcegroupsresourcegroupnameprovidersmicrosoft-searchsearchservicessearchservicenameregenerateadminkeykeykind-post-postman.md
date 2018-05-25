{
  "info": {
    "name": "Azure Search API Admin Keys Regenerate",
    "_postman_id": "7f4c9038-39b8-4a01-b832-220924c69b8c",
    "description": "Regenerates either the primary or secondary admin API key. You can only regenerate one key at a time.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "admin keys",
      "item": [
        {
          "id": "f28e8d36-3f47-48ed-8efe-2bb06e706ada",
          "name": "AdminKeys_Regenerate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Search/searchServices/:searchServiceName/regenerateAdminKey/:keyKind"
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
                  "id": "keyKind",
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
            "description": "Regenerates either the primary or secondary admin API key"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71276090-1caf-4887-8acc-af6f5e4faa4a"
            }
          ]
        }
      ]
    }
  ]
}