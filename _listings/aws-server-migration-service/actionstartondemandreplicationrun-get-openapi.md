---
swagger: "2.0"
x-collection-name: AWS Server Migration Service
x-complete: 0
info:
  title: AWS Server Migration Service API Start On Demand Replication Run
  version: 1.0.0
  description: The start-on-demand-replication-run API is used to start a ReplicationRun
    on demand (in addition to those that are scheduled based on your frequency).
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartOnDemandReplicationRun:
    get:
      summary: Start On Demand Replication Run
      description: The start-on-demand-replication-run API is used to start a ReplicationRun
        on demand (in addition to those that are scheduled based on your frequency).
      operationId: startOnDemandReplicationRun
      x-api-path-slug: actionstartondemandreplicationrun-get
      parameters:
      - in: query
        name: description
        description: 'Type: String'
        type: string
      - in: query
        name: replicationJobId
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Runs
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