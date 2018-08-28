{
  "info": {
    "name": "Dezrez Get a list of special arrangements for a property",
    "_postman_id": "625e9210-60d9-49aa-b88a-28397ac72eaf",
    "description": "Get a list of special arrangements for a property.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "e702ec42-8456-4c9f-8261-f33358837c90",
          "name": "Property_SpecialArrangementsByid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/property/:id/specialarrangements"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of special arrangements for a property."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c8faed7-7093-416d-bec1-9c2c90dd40e3"
            }
          ]
        }
      ]
    }
  ]
}