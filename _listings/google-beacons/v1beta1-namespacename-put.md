---
swagger: "2.0"
info:
  title: Google Proximity Beacon
  description: Registers, manages, indexes, and searches beacons.
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
  /v1beta1/{namespaceName}:
    put:
      summary: Update Namespace
      description: Updates the information about the specified namespace
      operationId: proximitybeacon.namespaces.update
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: namespaceName
        description: Resource name of this namespace
      - in: query
        name: projectId
        description: The project id of the namespace to update
      responses:
        200:
          description: OK
      tags:
      - namespace
definitions:
  AdvertisedId:
    properties:
      id:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
  AttachmentInfo:
    properties:
      data:
        description: This is a default description.
        type: put
      namespacedType:
        description: This is a default description.
        type: put
  Beacon:
    properties:
      beaconName:
        description: This is a default description.
        type: put
      description:
        description: This is a default description.
        type: put
      expectedStability:
        description: This is a default description.
        type: put
      placeId:
        description: This is a default description.
        type: put
      properties:
        description: This is a default description.
        type: put
      provisioningKey:
        description: This is a default description.
        type: put
      status:
        description: This is a default description.
        type: put
  BeaconAttachment:
    properties:
      attachmentName:
        description: This is a default description.
        type: put
      creationTimeMs:
        description: This is a default description.
        type: put
      data:
        description: This is a default description.
        type: put
      namespacedType:
        description: This is a default description.
        type: put
  BeaconInfo:
    properties:
      attachments:
        description: This is a default description.
        type: put
      beaconName:
        description: This is a default description.
        type: put
  Date:
    properties:
      day:
        description: This is a default description.
        type: put
      month:
        description: This is a default description.
        type: put
      year:
        description: This is a default description.
        type: put
  DeleteAttachmentsResponse:
    properties:
      numDeleted:
        description: This is a default description.
        type: put
  Diagnostics:
    properties:
      alerts:
        description: This is a default description.
        type: put
      beaconName:
        description: This is a default description.
        type: put
  Empty:
    properties: []
  EphemeralIdRegistration:
    properties:
      beaconEcdhPublicKey:
        description: This is a default description.
        type: put
      beaconIdentityKey:
        description: This is a default description.
        type: put
      initialClockValue:
        description: This is a default description.
        type: put
      initialEid:
        description: This is a default description.
        type: put
      rotationPeriodExponent:
        description: This is a default description.
        type: put
      serviceEcdhPublicKey:
        description: This is a default description.
        type: put
  EphemeralIdRegistrationParams:
    properties:
      maxRotationPeriodExponent:
        description: This is a default description.
        type: put
      minRotationPeriodExponent:
        description: This is a default description.
        type: put
      serviceEcdhPublicKey:
        description: This is a default description.
        type: put
  GetInfoForObservedBeaconsRequest:
    properties:
      namespacedTypes:
        description: This is a default description.
        type: put
      observations:
        description: This is a default description.
        type: put
  GetInfoForObservedBeaconsResponse:
    properties:
      beacons:
        description: This is a default description.
        type: put
  IndoorLevel:
    properties:
      name:
        description: This is a default description.
        type: put
  LatLng:
    properties:
      latitude:
        description: This is a default description.
        type: put
      longitude:
        description: This is a default description.
        type: put
  ListBeaconAttachmentsResponse:
    properties:
      attachments:
        description: This is a default description.
        type: put
  ListBeaconsResponse:
    properties:
      beacons:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
      totalCount:
        description: This is a default description.
        type: put
  ListDiagnosticsResponse:
    properties:
      diagnostics:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  ListNamespacesResponse:
    properties:
      namespaces:
        description: This is a default description.
        type: put
  Namespace:
    properties:
      namespaceName:
        description: This is a default description.
        type: put
      servingVisibility:
        description: This is a default description.
        type: put
  Observation:
    properties:
      telemetry:
        description: This is a default description.
        type: put
      timestampMs:
        description: This is a default description.
        type: put
x-collection-name: Google Beacons
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