---
name: Plentymarkets
x-slug: plentymarkets
description: plentymarkets is an all-in-one e-commerce ERP solution, which combines
  a comprehensive stock management system with a versatile shop system and effortless
  multichannel sales. Thanks to comprehensive functions and interfaces that include
  all steps of the e-commerce value chain, you can use the cloud based software to
  completely automate all of your e-business processes as well as your companys own
  individual processes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
x-kinRank: "7"
x-alexaRank: ""
tags: VAT
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/vat/master/_listings/plentymarkets/apis.md
specificationVersion: "0.14"
apis:
- name: plentymarkets REST-API - List VAT configurations.
  x-api-slug: restvat-get
  description: Lists the VAT configurations for the given filter. Possible filters
    are <code>locationId</code>, <code>countryId</code>, <code>taxIdNumber</code>
    and <code>startedAt</code>.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vat/master/_listings/plentymarkets/restvat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vat/master/_listings/plentymarkets/restvat-get-openapi.md
- name: plentymarkets REST-API - Create a VAT configuration
  x-api-slug: restvat-post
  description: Create a vat configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vat/master/_listings/plentymarkets/restvat-post-openapi.md
- name: plentymarkets REST-API - List VAT configurations of an accounting location
  x-api-slug: restvatlocationslocationid-get
  description: Lists the VAT configurations for all countries of one accounting location
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vat/master/_listings/plentymarkets/restvatlocationslocationid-get-openapi.md
- name: plentymarkets REST-API - List VAT configurations for one country of delivery
  x-api-slug: restvatlocationslocationidcountriescountryid-get
  description: Lists the VAT configurations for a country of delivery of one accounting
    location. The ID of the accounting location and the ID of the country of delivery
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vat/master/_listings/plentymarkets/restvatlocationslocationidcountriescountryid-get-openapi.md
- name: plentymarkets REST-API - Get a VAT configuration for a country in a location.
  x-api-slug: restvatlocationslocationidcountriescountryiddatedate-get
  description: Gets the VAT configuration found by matching the given location, delivery
    country and date of validity.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vat/master/_listings/plentymarkets/restvatlocationslocationidcountriescountryiddatedate-get-openapi.md
- name: plentymarkets REST-API - Get a VAT configuration for the standard accounting
    location of a client
  x-api-slug: restvatstandard-get
  description: Gets the VAT configuration currently used for the country of the standard
    accounting location of a client (store). The ID of the client (store) must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vat/master/_listings/plentymarkets/restvatstandard-get-openapi.md
- name: plentymarkets REST-API - Get a VAT configuration by id
  x-api-slug: restvatvatid-get
  description: Get a vat configuration by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vat/master/_listings/plentymarkets/restvatvatid-get-openapi.md
- name: plentymarkets REST-API - Update a VAT configuration
  x-api-slug: restvatvatid-put
  description: Update a vat configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/vat/master/_listings/plentymarkets/restvatvatid-put-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.plentymarkets.co.uk/?ActionCall=WebActionRSS&rrss_id=1
- type: x-github
  url: https://github.com/plentymarkets
- type: x-twitter
  url: https://twitter.com/plentymarketsuk
- type: x-website
  url: http://www.plentymarkets.co.uk
- type: x-api-gallery
  url: http://pivotal.tracker.api.gallery.streamdata.io
- type: x-api-stack
  url: http://plentymarkets.stack.network
- type: x-blog
  url: https://www.plentymarkets.co.uk/blog/
- type: x-pricing
  url: https://www.plentymarkets.co.uk/prices/
- type: x-website
  url: https://www.plentymarkets.co.uk
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---