---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetCorporateIntradayVWAP:
    get:
      summary: Get Corporate Intraday VWAP
      description: Returns a corporate intraday VWAP for a security based on the trades
        performed in a time range.
      operationId: GetCorporateIntradayVWAP
      x-api-path-slug: getcorporateintradayvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Corporate
      - Intraday
      - VWAP
  /GetCorporateHistoricalVWAP:
    get:
      summary: Get Corporate Historical VWAP
      description: Returns a corporate intraday VWAP for a security based on the trades
        performed in a time range.
      operationId: GetCorporateHistoricalVWAP
      x-api-path-slug: getcorporatehistoricalvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Corporate
      - Historical
      - VWAP
---