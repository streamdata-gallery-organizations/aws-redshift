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
  /?Action=DeleteClusterSubnetGroup&k=1:
    get:
      summary: ' Delete Cluster Subnet Group '
      description: Deletes the specified cluster subnet group
      operationId: deleteClusterSubnetGroup
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name of the cluster subnet group name to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - cluster subnet groups
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