{
  "info": {
    "name": "Plentymarkets List VAT configurations.",
    "_postman_id": "4364663a-c8fc-4f6b-8e0f-2d1130ffa8ae",
    "description": "Lists the VAT configurations for the given filter. Possible filters are <code>locationId</code>, <code>countryId</code>, <code>taxIdNumber</code> and <code>startedAt</code>.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "28a367f6-4cf7-4eb2-901e-6834ec4f747c",
          "name": "getRestAccountingLocationsRevenueAccountConfigurations",
          "request": {
            "url": "http://example.com/rest/accounting/locations/revenue_account_configurations?itemsPerPage=%7B%7D&page=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists revenue account configurations of a system. The revenue accounts are returned as paginated result. By default 50 revenue accounts are on one page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b858e982-a82c-4566-8143-872a1ababd53"
            }
          ]
        },
        {
          "id": "6d93db83-5e28-4167-8439-d34f25439dd8",
          "name": "getRestVat",
          "request": {
            "url": "http://example.com/rest/vat?columns=%7B%7D&itemsPerPage=%7B%7D&page=%7B%7D&with=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists the VAT configurations for the given filter. Possible filters are <code>locationId</code>, <code>countryId</code>, <code>taxIdNumber</code> and <code>startedAt</code>."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66c7ef3b-6c0b-428a-89b0-bb2a8421783a"
            }
          ]
        }
      ]
    }
  ]
}