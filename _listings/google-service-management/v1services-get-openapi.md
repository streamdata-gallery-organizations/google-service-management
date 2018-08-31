---
swagger: "2.0"
x-collection-name: Google Service Management
x-complete: 0
info:
  title: Google Service Management API Get Services
  description: |-
    Lists managed services.

    Returns all public services. For authenticated users, also returns all
    services the calling user has "servicemanagement.services.get" permission
    for.

    **BETA:** If the caller specifies the `consumer_id`, it returns only the
    services enabled on the consumer. The `consumer_id` must have the format
    of "project:{PROJECT-ID}".
  contact:
    name: Google
    url: https://google.com
  version: v1
host: servicemanagement.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/services:
    get:
      summary: Get Services
      description: |-
        Lists managed services.

        Returns all public services. For authenticated users, also returns all
        services the calling user has "servicemanagement.services.get" permission
        for.

        **BETA:** If the caller specifies the `consumer_id`, it returns only the
        services enabled on the consumer. The `consumer_id` must have the format
        of "project:{PROJECT-ID}".
      operationId: servicemanagement.services.list
      x-api-path-slug: v1services-get
      parameters:
      - in: query
        name: consumerId
        description: Include services consumed by the specified consumer
      - in: query
        name: pageSize
        description: Requested size of the next page of data
      - in: query
        name: pageToken
        description: Token identifying which result to start with; returned by a previous
          listcall
      - in: query
        name: producerProjectId
        description: Include services produced by the specified project
      responses:
        200:
          description: OK
      tags:
      - Service
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