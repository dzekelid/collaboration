---
name: SAP
x-slug: sap
description: Get software and technology solutions from SAP, the leader in business
  applications.  Run simple with the best in cloud, analytics, mobile and IT solutions.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
x-kinRank: "8"
x-alexaRank: "1965"
tags: Collaboration
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/apis.md
specificationVersion: "0.14"
apis:
- name: Manufacturing Network Customer APIs - Creates a collaboration room
  x-api-slug: collaborationrooms-post
  description: "Creates a collaboration room.  \nThe login user must be from a customer."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/collaborationrooms-post-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves a collaboration room
  x-api-slug: collaborationroomscollaborationroomid-get
  description: Retrieves the information of a collaboration room by its ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/collaborationroomscollaborationroomid-get-openapi.md
- name: Manufacturing Network Customer APIs - Updates a collaboration room
  x-api-slug: collaborationroomscollaborationroomid-patch
  description: Updates a collaboration room.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/collaborationroomscollaborationroomid-patch-openapi.md
- name: Manufacturing Network Customer APIs - Deletes a collaboration room
  x-api-slug: collaborationroomscollaborationroomid-delete
  description: |-
    Deletes a collaboration room
    The login user must be a collaboration lead for the customer and it must be a new or discarded collaboration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/collaborationroomscollaborationroomid-delete-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves basic info of a collaboration
    room
  x-api-slug: collaborationroomscollaborationroomidbasic-get
  description: Retrieves the information of a collaboration room in a simplified form.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/collaborationroomscollaborationroomidbasic-get-openapi.md
- name: Manufacturing Network Customer APIs - Starts a collaboration
  x-api-slug: collaborationroomscollaborationroomidstart-post
  description: "Sets a collaboration in process.  \nThe collaboration must be a new
    collaboration."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/collaborationroomscollaborationroomidstart-post-openapi.md
- name: Manufacturing Network Customer APIs - Completes a collaboration
  x-api-slug: collaborationroomscollaborationroomidcomplete-post
  description: |-
    Sets a collaboration as completed
    - The login user must be a collaboration lead for the customer.
    - If there's already a supplier in the collaboration room, the collaboration must already or still be in process.
    - If there's already a completed collaboration with the same additive manufacturing supplier, part ID, and customer, this operation fails.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/collaborationroomscollaborationroomidcomplete-post-openapi.md
- name: Manufacturing Network Customer APIs - Discards a collaboration
  x-api-slug: collaborationroomscollaborationroomiddiscard-post
  description: "Sets a collaboration as discarded.  \nThe login user must be a collaboration
    lead for the customer and the collaboration must be in process or completed."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/collaborationroomscollaborationroomiddiscard-post-openapi.md
- name: Manufacturing Network Customer APIs - Reopens a collaboration
  x-api-slug: collaborationroomscollaborationroomidreopen-post
  description: "Reopens a completed collaboration.  \nThe collaboration is set back
    to the status 'In Process'.\nThe login user must be a collaboration lead for the
    customer."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/collaborationroomscollaborationroomidreopen-post-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves documents in a collaboration
    room
  x-api-slug: collaborationroomscollaborationroomiddocuments-get
  description: Retrieves the information of all documents in a collaboration room,
    such as design files and specifications.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/collaborationroomscollaborationroomiddocuments-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves available collaboration room
    templates
  x-api-slug: collaborationtemplates-get
  description: Retrieves available collaboration room templates.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/collaborationtemplates-get-openapi.md
- name: Manufacturing Network Customer APIs - Uploads a file to a collaboration room
  x-api-slug: documentscollaborationroomscollaborationroomidupload-post
  description: Uploads a file to a collaboration room.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/documentscollaborationroomscollaborationroomidupload-post-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves the collaboration rooms of
    an organization
  x-api-slug: organizationsorganizationidcollaborationrooms-get
  description: "Retrieves the collaboration rooms where the login user's organization
    is a collaboration party.   \n- If the login user is not an organization admin,
    only the collaboration rooms where the login user is a participant are retrieved.
    \  \n- If the login user is an organization admin, all the collaboration rooms
    where the login user's organization is a collaboration party are retrieved. The
    login user may not be part of the collaborations."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/organizationsorganizationidcollaborationrooms-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves the collaboration rooms created
    by an organization
  x-api-slug: organizationsorganizationidcollaborationroomsowned-get
  description: "Retrieves the collaboration rooms created and owned by an organization.
    \ \n- If the login user is not an organization admin, only the collaboration rooms
    where the login user is a participant are retrieved.  \n- If the login user is
    an organization admin, all the collaboration rooms owned by the login user's organization
    are retrieved."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/organizationsorganizationidcollaborationroomsowned-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves collaboration room template
    types
  x-api-slug: templatetypes-get
  description: Retrieves available collaboration room template types.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/templatetypes-get-openapi.md
- name: Manufacturing Network Customer APIs - Retrieves a user's collaboration rooms
  x-api-slug: usersuseridcollaborationrooms-get
  description: "Retrieves the collaboration rooms where a user is a participant.  \n-
    If the login user is not an organization admin, he or she can search only by his
    or her own user ID and retrieve the collaboration rooms where he or she is a participant.
    \ \n- If the login user is an organization admin, he or she can search by the
    user ID of any user in the same organization."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/usersuseridcollaborationrooms-get-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves a collaboration room
  x-api-slug: collaborationroomscollaborationroomid-get
  description: Retrieves the information of a collaboration room by its ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/collaborationroomscollaborationroomid-get-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves basic info of a collaboration
    room
  x-api-slug: collaborationroomscollaborationroomidbasic-get
  description: Retrieves the information of a collaboration room in a simplified form.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/collaborationroomscollaborationroomidbasic-get-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves documents in a collaboration
    room
  x-api-slug: collaborationroomscollaborationroomiddocuments-get
  description: Retrieves the information of all documents in a collaboration room,
    such as design files and specifications.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/collaborationroomscollaborationroomiddocuments-get-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves the collaboration rooms of
    an organization
  x-api-slug: organizationsorganizationidcollaborationrooms-get
  description: Retrieves the collaboration rooms where an organization is a collaboration
    party.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/organizationsorganizationidcollaborationrooms-get-openapi.md
- name: Manufacturing Network Partner APIs - Retrieves the collaboration rooms created
    by an organization
  x-api-slug: organizationsorganizationidcollaborationroomsowned-get
  description: Retrieves the collaboration rooms created and owned by an organization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28252-www-sap-com.jpg
  humanURL: https://www.sap.com/index.html
  baseURL: https://hostname//dim/api
  tags: SaaS, Technology, Enterprise, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/collaboration/master/_listings/sap/organizationsorganizationidcollaborationroomsowned-get-openapi.md
x-common:
- type: x-website
  url: https://www.sap.com/index.html
- type: x-api-gallery
  url: http://santander.bank.api.gallery.streamdata.io
- type: x-api-stack
  url: http://sap.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/sap-canada
- type: x-developer
  url: https://api.sap.com/
- type: x-github
  url: https://github.com/sap
- type: x-twitter
  url: https://twitter.com/SAP
- type: x-website
  url: https://www.sap.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---