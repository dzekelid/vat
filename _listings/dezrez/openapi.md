---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/agency/getvatrate:
    get:
      summary: Gets the current VAT rate unless the date is specified
      description: Gets the current vat rate unless the date is specified.
      operationId: Agency_GetVatRateByvatRateTypeByvatDate
      x-api-path-slug: apiagencygetvatrate-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: vatDate
        description: Date of VAT value, used to get historic or future VAT Rates
      - in: query
        name: vatRateType
        description: Vat Rate type, standard is currently option
      responses:
        200:
          description: OK
      tags:
      - S
      - Current
      - VAT
      - Rate
      - Unless
      - Date
      - Is
      - Specified
---