---
swagger: "2.0"
x-collection-name: uebermaps
x-complete: 1
info:
  title: uebermaps
  description: enable-people-to-store-spots-on-public-and-private-maps
  termsOfService: https://uebermaps.com/terms/
  contact:
    name: uebermaps API Team
  version: "2.0"
host: uebermaps.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /maps/{id}/collaborators/{user_id}:
    delete:
      summary: Delete collaboration
      description: Delete collaboration.
      operationId: maps.id.collaborators.user_id.delete
      x-api-path-slug: mapsidcollaboratorsuser-id-delete
      parameters:
      - in: path
        name: id
        description: map id
      - in: path
        name: user_id
        description: user id
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Collaboration
---