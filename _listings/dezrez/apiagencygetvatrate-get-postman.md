{
  "info": {
    "name": "Dezrez Gets the current VAT rate unless the date is specified",
    "_postman_id": "46c60a07-65c4-463f-9f86-fedd67de84a8",
    "description": "Gets the current vat rate unless the date is specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "S",
      "item": [
        {
          "id": "559d6ade-fcbc-4732-bab9-240842f69689",
          "name": "Agency_GetVatRateByvatRateTypeByvatDate",
          "request": {
            "url": "http://api.dezrez.com/api/agency/getvatrate?vatDate=%7B%7D&vatRateType=%7B%7D",
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
            "description": "Gets the current vat rate unless the date is specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b222bb2e-3b02-46eb-9c6c-96f86c3b1683"
            }
          ]
        }
      ]
    }
  ]
}