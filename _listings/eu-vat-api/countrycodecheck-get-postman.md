{
  "info": {
    "name": "EU VAT API Retrieve a countries VAT rates by its 2 digit country code",
    "_postman_id": "385019a4-ba8d-4524-a504-f59bfb616bce",
    "description": "Retrieve a countries vat rates by its 2 digit country code.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Retrieve",
      "item": [
        {
          "id": "254de7f1-bce1-4179-a9cd-443df93eff50",
          "name": "country_code_check",
          "request": {
            "url": "http://vatapi.com/v1/country-code-check?code=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Response-Type",
                "value": "{}",
                "description": "The default response type is application/json if you would like to receive an XML response then set this to XML",
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
            "description": "Retrieve a countries vat rates by its 2 digit country code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1dd61406-7ba6-4aea-b7eb-8ce85c8451ea"
            }
          ]
        }
      ]
    }
  ]
}