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
  /?Action=CreateHsmClientCertificate&k=1:
    get:
      summary: ' Create Hsm Client Certificate '
      description: |-
        Creates an HSM client certificate that an Amazon Redshift cluster will use to connect to
                    the client's HSM in order to store and retrieve the keys used to encrypt the cluster
                    databases
      operationId: createHsmClientCertificate
      parameters:
      - in: query
        name: HsmClientCertificateIdentifier
        description: The identifier to be assigned to the new HSM client certificate
          that the cluster            will use to connect to the HSM to use the database
          encryption keys
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - hsm client certificates
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