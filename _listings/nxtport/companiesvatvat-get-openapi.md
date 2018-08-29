---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 0
info:
  title: Port+ Portdirectory API Get Companies Vat Vat
  description: Get a company by its vat.
  version: 1.0.0
host: api.nxtport.eu
basePath: /portdirectory/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /companies/vat/{vat}:
    get:
      summary: Get Companies Vat Vat
      description: Get a company by its vat.
      operationId: Company_GetCompanyByVat
      x-api-path-slug: companiesvatvat-get
      parameters:
      - in: path
        name: vat
        description: Vat of the company
      responses:
        200:
          description: OK
      tags:
      - Companies
      - Vat
      - Vat
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