---
swagger: "2.0"
x-collection-name: AWS Step Functions
x-complete: 0
info:
  title: AWS Step Functions API Start Execution
  version: 1.0.0
  description: Starts a state machine execution.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartExecution:
    get:
      summary: Start Execution
      description: Starts a state machine execution.
      operationId: startExecution
      x-api-path-slug: actionstartexecution-get
      parameters:
      - in: query
        name: input
        description: The JSON input data for the execution
        type: string
      - in: query
        name: name
        description: The name of the execution
        type: string
      - in: query
        name: stateMachineArn
        description: The Amazon Resource Name (ARN) of the state machine to execute
        type: string
      responses:
        200:
          description: OK
      tags:
      - State Machine
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