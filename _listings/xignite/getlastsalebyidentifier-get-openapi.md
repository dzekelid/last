---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite NASDAQ Last Sale Get Last Sale By Identifier
  description: Returns a real-time quote for a security based on the last trade execution.
  version: 1.0.0
host: nasdaqlastsale.xignite.com
basePath: xNASDAQLastSale.json/XigniteNASDAQLastSale
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetLastSale:
    get:
      summary: Get Last Sale
      description: Returns real time stock quote for a given stock ticker
      operationId: GetLastSale
      x-api-path-slug: getlastsale-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Last
      - Sale
  /GetLastSales:
    get:
      summary: Get Last Sales
      description: Returns a collection of real time stock quotes for a comma-separated
        list of stock quotes.
      operationId: GetLastSales
      x-api-path-slug: getlastsales-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Last
      - Sales
  /GetLastIndustryHeadlines:
    get:
      summary: Get Last Industry Headlines
      description: Return the last press releases since a certain time for an industry.
      operationId: postGetlastindustryheadlines
      x-api-path-slug: getlastindustryheadlines-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Last
      - Industry
      - Headlines
  /GetGlobalLastClosingPrice:
    get:
      summary: Get Global Last Closing Price
      description: Returns last closing price for a security.
      operationId: postGetgloballastclosingprice
      x-api-path-slug: getgloballastclosingprice-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Global
      - Last
      - Closing
      - Price
  /GetGlobalLastClosingPrices:
    get:
      summary: Get Global Last Closing Prices
      description: Returns last closing price for a collection of securities.
      operationId: postGetgloballastclosingprices
      x-api-path-slug: getgloballastclosingprices-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Global
      - Last
      - Closing
      - Prices
  /GetLastClosingIndicesValue:
    get:
      summary: Get Last Closing Indices Value
      description: Get last closing indices value.
      operationId: GetLastClosingIndicesValue
      x-api-path-slug: getlastclosingindicesvalue-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Last
      - Closing
      - Indices
      - Value
  /GetLastClosingIndexValue:
    get:
      summary: Get Last Closing Index Value
      description: Get last closing index value.
      operationId: GetLastClosingIndexValue
      x-api-path-slug: getlastclosingindexvalue-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Last
      - Closing
      - Index
      - Value
  /GetLastClosingPrice:
    get:
      summary: Get Last Closing Price
      description: Returns last closing price for a security.
      operationId: postGetlastclosingprice
      x-api-path-slug: getlastclosingprice-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Last
      - Closing
      - Price
  /GetLastClosingPriceAdjusted:
    get:
      summary: Get Last Closing Price Adjusted
      description: Returns last closing price for a security. This include the splits
        and dividends adjusted price
      operationId: postGetlastclosingpriceadjusted
      x-api-path-slug: getlastclosingpriceadjusted-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Last
      - Closing
      - Price
      - Adjusted
  /GetLastClosingPrices:
    get:
      summary: Get Last Closing Prices
      description: Returns last closing price for a collection of securities.
      operationId: postGetlastclosingprices
      x-api-path-slug: getlastclosingprices-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Last
      - Closing
      - Prices
  /GetLastClosingPricesAdjusted:
    get:
      summary: Get Last Closing Prices Adjusted
      description: Returns last closing price for a collection of securities.This
        include the splits and dividends adjusted price
      operationId: postGetlastclosingpricesadjusted
      x-api-path-slug: getlastclosingpricesadjusted-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Last
      - Closing
      - Prices
      - Adjusted
  /GetLastClosingPricesOrdered:
    get:
      summary: Get Last Closing Prices Ordered
      description: Returns last closing price for a collection of securities.
      operationId: postGetlastclosingpricesordered
      x-api-path-slug: getlastclosingpricesordered-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Last
      - Closing
      - Prices
      - Ordered
  /GetLastClosingPricesOrderedAdjusted:
    get:
      summary: Get Last Closing Prices Ordered Adjusted
      description: Returns last closing price for a collection of securities.This
        include the splits and dividends adjusted price
      operationId: postGetlastclosingpricesorderedadjusted
      x-api-path-slug: getlastclosingpricesorderedadjusted-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Last
      - Closing
      - Prices
      - Ordered
      - Adjusted
  /GetLastSaleByIdentifier:
    get:
      summary: Get Last Sale By Identifier
      description: Returns a real-time quote for a security based on the last trade
        execution.
      operationId: GetLastSaleByIdentifier
      x-api-path-slug: getlastsalebyidentifier-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Last
      - Sale
      - Identifier
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