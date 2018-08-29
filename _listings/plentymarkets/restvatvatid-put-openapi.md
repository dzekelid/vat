---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Update a VAT configuration
  description: Update a vat configuration.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/vat:
    get:
      summary: List VAT configurations.
      description: Lists the VAT configurations for the given filter. Possible filters
        are <code>locationId</code>, <code>countryId</code>, <code>taxIdNumber</code>
        and <code>startedAt</code>.
      operationId: getRestVat
      x-api-path-slug: restvat-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: with
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - List
      - VAT
      - Configurations
    post:
      summary: Create a VAT configuration
      description: Create a vat configuration.
      operationId: postRestVat
      x-api-path-slug: restvat-post
      parameters:
      - in: body
        name: /rest/vat
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configuration
  /rest/vat/locations/{locationId}:
    get:
      summary: List VAT configurations of an accounting location
      description: Lists the VAT configurations for all countries of one accounting
        location
      operationId: getRestVatLocationsLocation
      x-api-path-slug: restvatlocationslocationid-get
      parameters:
      - in: query
        name: columns[]
        description: The attributes of the VAT configuration
      - in: path
        name: locationId
      - in: query
        name: with[]
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - List
      - VAT
      - Configurations
      - Of
      - Accounting
      - Location
  /rest/vat/locations/{locationId}/countries/{countryId}:
    get:
      summary: List VAT configurations for one country of delivery
      description: Lists the VAT configurations for a country of delivery of one accounting
        location. The ID of the accounting location and the ID of the country of delivery
        must be specified.
      operationId: getRestVatLocationsLocationCountriesCountry
      x-api-path-slug: restvatlocationslocationidcountriescountryid-get
      parameters:
      - in: query
        name: columns[]
        description: The attributes of the VAT configuration
      - in: path
        name: countryId
      - in: path
        name: locationId
      - in: query
        name: with[]
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - List
      - VAT
      - Configurationsone
      - Country
      - Of
      - Delivery
  /rest/vat/locations/{locationId}/countries/{countryId}/date/{date}:
    get:
      summary: Get a VAT configuration for a country in a location.
      description: Gets the VAT configuration found by matching the given location,
        delivery country and date of validity.
      operationId: getRestVatLocationsLocationCountriesCountryDateDate
      x-api-path-slug: restvatlocationslocationidcountriescountryiddatedate-get
      parameters:
      - in: query
        name: columns[]
        description: The attributes of the VAT configuration
      - in: path
        name: countryId
      - in: path
        name: date
      - in: path
        name: locationId
      - in: query
        name: startDate
        description: The date of validity
      - in: query
        name: with[]
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configurationa
      - Country
      - In
      - Location
  /rest/vat/standard:
    get:
      summary: Get a VAT configuration for the standard accounting location of a client
      description: Gets the VAT configuration currently used for the country of the
        standard accounting location of a client (store). The ID of the client (store)
        must be specified.
      operationId: getRestVatStandard
      x-api-path-slug: restvatstandard-get
      parameters:
      - in: query
        name: plentyId
        description: The plenty ID of the client (store)
      - in: query
        name: startedAt
        description: The date in the W3C format when the vat configuration went into
          effect
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configurationthe
      - Standard
      - Accounting
      - Location
      - Of
      - Client
  /rest/vat/{vatId}:
    get:
      summary: Get a VAT configuration by id
      description: Get a vat configuration by id.
      operationId: getRestVatVat
      x-api-path-slug: restvatvatid-get
      parameters:
      - in: path
        name: vatId
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configuration
      - By
      - Id
    put:
      summary: Update a VAT configuration
      description: Update a vat configuration.
      operationId: putRestVatVat
      x-api-path-slug: restvatvatid-put
      parameters:
      - in: body
        name: /rest/vat/{vatId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: vatId
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configuration
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