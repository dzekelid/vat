---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Get a VAT configuration for a country in a location.
  description: Gets the VAT configuration found by matching the given location, delivery
    country and date of validity.
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