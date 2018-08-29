---
swagger: "2.0"
x-collection-name: Taxamo
x-complete: 0
info:
  title: Taxamo Validate VAT Number
  description: Validate vat number.
  version: "1"
host: api.taxamo.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/tax/vat_numbers/{tax_number}/validate:
    get:
      summary: Validate VAT Number
      description: Validate vat number.
      operationId: validateTaxNumber
      x-api-path-slug: apiv1taxvat-numberstax-numbervalidate-get
      parameters:
      - in: query
        name: country_code
        description: Two-letter ISO country code
      - in: path
        name: tax_number
        description: Tax number
      responses:
        200:
          description: OK
      tags:
      - Validate
      - VAT
      - Number
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---