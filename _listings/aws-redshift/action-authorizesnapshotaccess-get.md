---
swagger: "2.0"
info:
  title: AWS Redshift API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AuthorizeSnapshotAccess&k=1:
    get:
      summary: ' Authorize Snapshot Access '
      description: |-
        Authorizes the specified AWS customer account to restore the specified
                    snapshot
      operationId: authorizeSnapshotAccess
      parameters:
      - in: query
        name: AccountWithRestoreAccess
        description: The identifier of the AWS customer account authorized to restore
          the specified            snapshot
        type: string
      - in: query
        name: SnapshotClusterIdentifier
        description: The identifier of the cluster the snapshot was created from
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The identifier of the snapshot the account is authorized to restore
        type: string
      responses:
        200:
          description: OK
      tags:
      - snapshots
definitions: []
x-collection-name: AWS Redshift
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