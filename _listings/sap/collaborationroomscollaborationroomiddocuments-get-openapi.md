---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Manufacturing Network Partner APIs Retrieves documents in a collaboration
    room
  description: Retrieves the information of all documents in a collaboration room,
    such as design files and specifications.
  version: 1.0.0
host: hostname
basePath: /dim/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /collaborationRooms:
    post:
      summary: Creates a collaboration room
      description: "Creates a collaboration room.  \nThe login user must be from a
        customer."
      operationId: creates-a-collaboration-room--the-login-user-must-be-from-a-customer
      x-api-path-slug: collaborationrooms-post
      parameters:
      - in: body
        name: CollaborationRoomCreateRequest
        description: A request about creating a collaboration room
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - Collaboration
      - Room
  /collaborationRooms/{collaborationRoomId}:
    get:
      summary: Retrieves a collaboration room
      description: Retrieves the information of a collaboration room by its ID.
      operationId: retrieves-the-information-of-a-collaboration-room-by-its-id
      x-api-path-slug: collaborationroomscollaborationroomid-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Collaboration
      - Room
    patch:
      summary: Updates a collaboration room
      description: Updates a collaboration room.
      operationId: updates-a-collaboration-room
      x-api-path-slug: collaborationroomscollaborationroomid-patch
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: body
        name: CollaborationRoomUpdateRequest
        description: A request about updating a collaboration room
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Collaboration
      - Room
    delete:
      summary: Deletes a collaboration room
      description: |-
        Deletes a collaboration room
        The login user must be a collaboration lead for the customer and it must be a new or discarded collaboration.
      operationId: deletes-a-collaboration-roomthe-login-user-must-be-a-collaboration-lead-for-the-customer-and-it-must
      x-api-path-slug: collaborationroomscollaborationroomid-delete
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Collaboration
      - Room
  /collaborationRooms/{collaborationRoomId}/basic:
    get:
      summary: Retrieves basic info of a collaboration room
      description: Retrieves the information of a collaboration room in a simplified
        form.
      operationId: retrieves-the-information-of-a-collaboration-room-in-a-simplified-form
      x-api-path-slug: collaborationroomscollaborationroomidbasic-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Basic
      - Info
      - Of
      - Collaboration
      - Room
  /collaborationRooms/{collaborationRoomId}/start:
    post:
      summary: Starts a collaboration
      description: "Sets a collaboration in process.  \nThe collaboration must be
        a new collaboration."
      operationId: sets-a-collaboration-in-process--the-collaboration-must-be-a-new-collaboration
      x-api-path-slug: collaborationroomscollaborationroomidstart-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Starts
      - Collaboration
  /collaborationRooms/{collaborationRoomId}/complete:
    post:
      summary: Completes a collaboration
      description: |-
        Sets a collaboration as completed
        - The login user must be a collaboration lead for the customer.
        - If there's already a supplier in the collaboration room, the collaboration must already or still be in process.
        - If there's already a completed collaboration with the same additive manufacturing supplier, part ID, and customer, this operation fails.
      operationId: sets-a-collaboration-as-completed-the-login-user-must-be-a-collaboration-lead-for-the-customer-if-th
      x-api-path-slug: collaborationroomscollaborationroomidcomplete-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Completes
      - Collaboration
  /collaborationRooms/{collaborationRoomId}/discard:
    post:
      summary: Discards a collaboration
      description: "Sets a collaboration as discarded.  \nThe login user must be a
        collaboration lead for the customer and the collaboration must be in process
        or completed."
      operationId: sets-a-collaboration-as-discarded--the-login-user-must-be-a-collaboration-lead-for-the-customer-and-
      x-api-path-slug: collaborationroomscollaborationroomiddiscard-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Discards
      - Collaboration
  /collaborationRooms/{collaborationRoomId}/reopen:
    post:
      summary: Reopens a collaboration
      description: "Reopens a completed collaboration.  \nThe collaboration is set
        back to the status 'In Process'.\nThe login user must be a collaboration lead
        for the customer."
      operationId: reopens-a-completed-collaboration--the-collaboration-is-set-back-to-the-status-in-processthe-login-u
      x-api-path-slug: collaborationroomscollaborationroomidreopen-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Reopens
      - Collaboration
  /collaborationRooms/{collaborationRoomId}/documents:
    get:
      summary: Retrieves documents in a collaboration room
      description: Retrieves the information of all documents in a collaboration room,
        such as design files and specifications.
      operationId: retrieves-the-information-of-all-documents-in-a-collaboration-room-such-as-design-files-and-specific
      x-api-path-slug: collaborationroomscollaborationroomiddocuments-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Documents
      - In
      - Collaboration
      - Room
  /collaborationTemplates:
    get:
      summary: Retrieves available collaboration room templates
      description: Retrieves available collaboration room templates.
      operationId: retrieves-available-collaboration-room-templates
      x-api-path-slug: collaborationtemplates-get
      parameters:
      - in: query
        name: typeId
        description: The ID of a collaboration room template
      - in: query
        name: typeName
        description: The name of a collaboration room template
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Available
      - Collaboration
      - Room
      - Templates
  /documents/collaborationRooms/{collaborationRoomId}/upload:
    post:
      summary: Uploads a file to a collaboration room
      description: Uploads a file to a collaboration room.
      operationId: uploads-a-file-to-a-collaboration-room
      x-api-path-slug: documentscollaborationroomscollaborationroomidupload-post
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: formData
        name: fileUpload
        description: A file to be uploaded
      - in: formData
        name: originFileDisplay
        description: Indicates if a file is visible to all participants in the collaboration
          room (public) or to the uploader only (private)
      responses:
        200:
          description: Successful response
      tags:
      - Uploads
      - File
      - To
      - Collaboration
      - Room
  /organizations/{organizationId}/collaborationRooms:
    get:
      summary: Retrieves the collaboration rooms of an organization
      description: "Retrieves the collaboration rooms where the login user's organization
        is a collaboration party.   \n- If the login user is not an organization admin,
        only the collaboration rooms where the login user is a participant are retrieved.
        \  \n- If the login user is an organization admin, all the collaboration rooms
        where the login user's organization is a collaboration party are retrieved.
        The login user may not be part of the collaborations."
      operationId: retrieves-the-collaboration-rooms-where-the-login-users-organization-is-a-collaboration-party----if-
      x-api-path-slug: organizationsorganizationidcollaborationrooms-get
      parameters:
      - in: path
        name: organizationId
        description: The ID of the login users organization
      - in: query
        name: organizationIds
        description: The IDs of other organizations
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Collaboration
      - Rooms
      - Of
      - Organization
  /organizations/{organizationId}/collaborationRooms/owned:
    get:
      summary: Retrieves the collaboration rooms created by an organization
      description: "Retrieves the collaboration rooms created and owned by an organization.
        \ \n- If the login user is not an organization admin, only the collaboration
        rooms where the login user is a participant are retrieved.  \n- If the login
        user is an organization admin, all the collaboration rooms owned by the login
        user's organization are retrieved."
      operationId: retrieves-the-collaboration-rooms-created-and-owned-by-an-organization---if-the-login-user-is-not-an
      x-api-path-slug: organizationsorganizationidcollaborationroomsowned-get
      parameters:
      - in: path
        name: organizationId
        description: The ID of the login users organization
      - in: query
        name: organizationIds
        description: The IDs of other organizations
      - in: query
        name: partId
        description: The ID of a part
      - in: query
        name: serviceType
        description: The type of service that a supplier organization provides during
          the collaboration
      - in: query
        name: status
        description: The status of a collaboration
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Collaboration
      - Rooms
      - Created
      - By
      - Organization
  /templateTypes:
    get:
      summary: Retrieves collaboration room template types
      description: Retrieves available collaboration room template types.
      operationId: retrieves-available-collaboration-room-template-types
      x-api-path-slug: templatetypes-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Collaboration
      - Room
      - Template
      - Types
  /users/{userId}/collaborationRooms:
    get:
      summary: Retrieves a user's collaboration rooms
      description: "Retrieves the collaboration rooms where a user is a participant.
        \ \n- If the login user is not an organization admin, he or she can search
        only by his or her own user ID and retrieve the collaboration rooms where
        he or she is a participant.  \n- If the login user is an organization admin,
        he or she can search by the user ID of any user in the same organization."
      operationId: retrieves-the-collaboration-rooms-where-a-user-is-a-participant---if-the-login-user-is-not-an-organi
      x-api-path-slug: usersuseridcollaborationrooms-get
      parameters:
      - in: path
        name: userId
        description: The ID of a user
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Users
      - Collaboration
      - Rooms
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