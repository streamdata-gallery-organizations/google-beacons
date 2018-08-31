---
name: Google Beacons
x-slug: google-beacons
description: Give your users better location and proximity experiences by providing
  a strong context signal for their devices in the form of Bluetooth low energy (BLE)
  beacons with Eddystone, the open beacon format from Google. The Google beacon platform
  enables you to manage your beacons remotely, integrate with Google services and
  help users devices to discover content and functionality across Android, native
  apps and the web.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
x-kinRank: "9"
x-alexaRank: "0"
tags: Google Beacons
created: "2018-08-30"
modified: "2018-08-30"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/apis.md
specificationVersion: "0.14"
apis:
- name: Google Proximity Beacon - Get Observed Beacon Info
  x-api-slug: v1beta1beaconinfogetforobserved-post
  description: |-
    Given one or more beacon observations, returns any beacon information
    and attachments accessible to your application. Authorize by using the
    [API key](https://developers.google.com/beacons/proximity/how-tos/authorizing#APIKey)
    for the application.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1beaconinfogetforobserved-post-openapi.md
- name: Google Proximity Beacon - Search Beacons
  x-api-slug: v1beta1beacons-get
  description: |-
    Searches the beacon registry for beacons that match the given search
    criteria. Only those beacons that the client has permission to list
    will be returned.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **viewer**, **Is owner** or **Can edit**
    permissions in the Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1beacons-get-openapi.md
- name: Google Proximity Beacon - Register Beacon
  x-api-slug: v1beta1beaconsregister-post
  description: |-
    Registers a previously unregistered beacon given its `advertisedId`.
    These IDs are unique within the system. An ID can be registered only once.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **Is owner** or **Can edit** permissions in the
    Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1beaconsregister-post-openapi.md
- name: Google Proximity Beacon - Get Beacon Parameters
  x-api-slug: v1beta1eidparams-get
  description: |-
    Gets the Proximity Beacon API's current public key and associated
    parameters used to initiate the Diffie-Hellman key exchange required to
    register a beacon that broadcasts the Eddystone-EID format. This key
    changes periodically; clients may cache it and re-use the same public key
    to provision and register multiple beacons. However, clients should be
    prepared to refresh this key when they encounter an error registering an
    Eddystone-EID beacon.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1eidparams-get-openapi.md
- name: Google Proximity Beacon - Get Namespace
  x-api-slug: v1beta1namespaces-get
  description: |-
    Lists all attachment namespaces owned by your Google Developers Console
    project. Attachment data associated with a beacon must include a
    namespaced type, and the namespace must be owned by your project.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **viewer**, **Is owner** or **Can edit**
    permissions in the Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1namespaces-get-openapi.md
- name: Google Proximity Beacon - Delete Attachment
  x-api-slug: v1beta1attachmentname-delete
  description: |-
    Deletes the specified attachment for the given beacon. Each attachment has
    a unique attachment name (`attachmentName`) which is returned when you
    fetch the attachment data via this API. You specify this with the delete
    request to control which attachment is removed. This operation cannot be
    undone.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **Is owner** or **Can edit** permissions in the
    Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1attachmentname-delete-openapi.md
- name: Google Proximity Beacon - Delete Beacon
  x-api-slug: v1beta1beaconname-delete
  description: |-
    Deletes the specified beacon including all diagnostics data for the beacon
    as well as any attachments on the beacon (including those belonging to
    other projects). This operation cannot be undone.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **Is owner** or **Can edit** permissions in the
    Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1beaconname-delete-openapi.md
- name: Google Proximity Beacon - Get Beacon
  x-api-slug: v1beta1beaconname-get
  description: |-
    Returns detailed information about the specified beacon.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **viewer**, **Is owner** or **Can edit**
    permissions in the Google Developers Console project.

    Requests may supply an Eddystone-EID beacon name in the form:
    `beacons/4!beaconId` where the `beaconId` is the base16 ephemeral ID
    broadcast by the beacon. The returned `Beacon` object will contain the
    beacon's stable Eddystone-UID. Clients not authorized to resolve the
    beacon's ephemeral Eddystone-EID broadcast will receive an error.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1beaconname-get-openapi.md
- name: Google Proximity Beacon - Update Beacon
  x-api-slug: v1beta1beaconname-put
  description: |-
    Updates the information about the specified beacon. **Any field that you do
    not populate in the submitted beacon will be permanently erased**, so you
    should follow the "read, modify, write" pattern to avoid inadvertently
    destroying data.

    Changes to the beacon status via this method will be  silently ignored.
    To update beacon status, use the separate methods on this API for
    activation, deactivation, and decommissioning.
    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **Is owner** or **Can edit** permissions in the
    Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1beaconname-put-openapi.md
- name: Google Proximity Beacon - Get Attachments
  x-api-slug: v1beta1beaconnameattachments-get
  description: |-
    Returns the attachments for the specified beacon that match the specified
    namespaced-type pattern.

    To control which namespaced types are returned, you add the
    `namespacedType` query parameter to the request. You must either use
    `*/*`, to return all attachments, or the namespace must be one of
    the ones returned from the  `namespaces` endpoint.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **viewer**, **Is owner** or **Can edit**
    permissions in the Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1beaconnameattachments-get-openapi.md
- name: Google Proximity Beacon - Add Attachment
  x-api-slug: v1beta1beaconnameattachments-post
  description: |-
    Associates the given data with the specified beacon. Attachment data must
    contain two parts:
    <ul>
    <li>A namespaced type.</li>
    <li>The actual attachment data itself.</li>
    </ul>
    The namespaced type consists of two parts, the namespace and the type.
    The namespace must be one of the values returned by the `namespaces`
    endpoint, while the type can be a string of any characters except for the
    forward slash (`/`) up to 100 characters in length.

    Attachment data can be up to 1024 bytes long.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **Is owner** or **Can edit** permissions in the
    Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1beaconnameattachments-post-openapi.md
- name: Google Proximity Beacon - Delete Attachments
  x-api-slug: v1beta1beaconnameattachmentsbatchdelete-post
  description: |-
    Deletes multiple attachments on a given beacon. This operation is
    permanent and cannot be undone.

    You can optionally specify `namespacedType` to choose which attachments
    should be deleted. If you do not specify `namespacedType`,  all your
    attachments on the given beacon will be deleted. You also may explicitly
    specify `*/*` to delete all.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **Is owner** or **Can edit** permissions in the
    Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1beaconnameattachmentsbatchdelete-post-openapi.md
- name: Google Proximity Beacon - Get Diagnostics
  x-api-slug: v1beta1beaconnamediagnostics-get
  description: |-
    List the diagnostics for a single beacon. You can also list diagnostics for
    all the beacons owned by your Google Developers Console project by using
    the beacon name `beacons/-`.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **viewer**, **Is owner** or **Can edit**
    permissions in the Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1beaconnamediagnostics-get-openapi.md
- name: Google Proximity Beacon - Activate Beacon
  x-api-slug: v1beta1beaconnameactivate-post
  description: |-
    Activates a beacon. A beacon that is active will return information
    and attachment data when queried via `beaconinfo.getforobserved`.
    Calling this method on an already active beacon will do nothing (but
    will return a successful response code).

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **Is owner** or **Can edit** permissions in the
    Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1beaconnameactivate-post-openapi.md
- name: Google Proximity Beacon - Deactivate Beacon
  x-api-slug: v1beta1beaconnamedeactivate-post
  description: |-
    Deactivates a beacon. Once deactivated, the API will not return
    information nor attachment data for the beacon when queried via
    `beaconinfo.getforobserved`. Calling this method on an already inactive
    beacon will do nothing (but will return a successful response code).

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **Is owner** or **Can edit** permissions in the
    Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1beaconnamedeactivate-post-openapi.md
- name: Google Proximity Beacon - Decomission Beacon
  x-api-slug: v1beta1beaconnamedecommission-post
  description: |-
    Decommissions the specified beacon in the service. This beacon will no
    longer be returned from `beaconinfo.getforobserved`. This operation is
    permanent -- you will not be able to re-register a beacon with this ID
    again.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **Is owner** or **Can edit** permissions in the
    Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1beaconnamedecommission-post-openapi.md
- name: Google Proximity Beacon - Update Namespace
  x-api-slug: v1beta1namespacename-put
  description: |-
    Updates the information about the specified namespace. Only the namespace
    visibility can be updated.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-beacons/master/_listings/google-beacons/v1beta1namespacename-put-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.apps.script.execution.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.beacons.stack.network
- type: x-dashboard
  url: https://developers.google.com/beacons/dashboard/
- type: x-website
  url: https://developers.google.com/beacons/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---