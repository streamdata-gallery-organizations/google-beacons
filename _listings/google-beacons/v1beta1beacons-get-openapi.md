---
swagger: "2.0"
x-collection-name: Google Beacons
x-complete: 0
info:
  title: Google Proximity Beacon API Search Beacons
  description: |-
    Searches the beacon registry for beacons that match the given search
    criteria. Only those beacons that the client has permission to list
    will be returned.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **viewer**, **Is owner** or **Can edit**
    permissions in the Google Developers Console project.
  contact:
    name: Google
    url: https://google.com
  version: v1beta1
host: proximitybeacon.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1beta1/beaconinfo:getforobserved:
    post:
      summary: Get Observed Beacon Info
      description: |-
        Given one or more beacon observations, returns any beacon information
        and attachments accessible to your application. Authorize by using the
        [API key](https://developers.google.com/beacons/proximity/how-tos/authorizing#APIKey)
        for the application.
      operationId: proximitybeacon.beaconinfo.getforobserved
      x-api-path-slug: v1beta1beaconinfogetforobserved-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Beacon
  /v1beta1/beacons:
    get:
      summary: Search Beacons
      description: |-
        Searches the beacon registry for beacons that match the given search
        criteria. Only those beacons that the client has permission to list
        will be returned.

        Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
        from a signed-in user with **viewer**, **Is owner** or **Can edit**
        permissions in the Google Developers Console project.
      operationId: proximitybeacon.beacons.list
      x-api-path-slug: v1beta1beacons-get
      parameters:
      - in: query
        name: pageSize
        description: The maximum number of records to return for this request, up
          to aserver-defined upper limit
      - in: query
        name: pageToken
        description: A pagination token obtained from a previous request to list beacons
      - in: query
        name: projectId
        description: The project id to list beacons under
      - in: query
        name: q
        description: 'Filter query string that supports the following field filters:*
          **description:``**  For example: **description:Room 3**  Returns beacons
          whose description matches tokens in the string Room 3  (not necessarily
          that exact string)'
      responses:
        200:
          description: OK
      tags:
      - Beacon
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