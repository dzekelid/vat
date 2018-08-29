swagger: "2.0"
x-collection-name: NxtPort
x-complete: 1
info:
  title: Portcall+ API (sandbox)
  description: portplus-api
  version: 1.0.0
host: api-sb.nxtport.eu
basePath: /PortCallPlus/v1
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