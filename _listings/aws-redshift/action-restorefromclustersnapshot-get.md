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
  /?Action=RestoreFromClusterSnapshot&k=1:
    get:
      summary: ' Restore From Cluster Snapshot '
      description: Creates a new cluster from a snapshot
      operationId: restoreFromClusterSnapshot
      parameters:
      - in: query
        name: AdditionalInfo
        description: Reserved
        type: string
      - in: query
        name: AllowVersionUpgrade
        description: If true, major version upgrades can be applied during the maintenance            window
          to the Amazon Redshift engine that is running on the cluster
        type: string
      - in: query
        name: AutomatedSnapshotRetentionPeriod
        description: The number of days that automated snapshots are retained
        type: string
      - in: query
        name: AvailabilityZone
        description: The Amazon EC2 Availability Zone in which to restore the cluster
        type: string
      - in: query
        name: ClusterIdentifier
        description: The identifier of the cluster that will be created from restoring
          the            snapshot
        type: string
      - in: query
        name: ClusterParameterGroupName
        description: The name of the parameter group to be associated with this cluster
        type: string
      - in: query
        name: ClusterSecurityGroups.ClusterSecurityGroupName.N
        description: A list of security groups to be associated with this cluster
        type: string
      - in: query
        name: ClusterSubnetGroupName
        description: The name of the subnet group where you want to cluster restored
        type: string
      - in: query
        name: ElasticIp
        description: The elastic IP (EIP) address for the cluster
        type: string
      - in: query
        name: EnhancedVpcRouting
        description: An option that specifies whether to create the cluster with enhanced
          VPC routing            enabled
        type: string
      - in: query
        name: HsmClientCertificateIdentifier
        description: Specifies the name of the HSM client certificate the Amazon Redshift
          cluster uses to            retrieve the data encryption keys stored in an
          HSM
        type: string
      - in: query
        name: HsmConfigurationIdentifier
        description: Specifies the name of the HSM configuration that contains the
          information the            Amazon Redshift cluster can use to retrieve and
          store keys in an HSM
        type: string
      - in: query
        name: IamRoles.IamRoleArn.N
        description: A list of AWS Identity and Access Management (IAM) roles that
          can be used by the            cluster to access other AWS services
        type: string
      - in: query
        name: KmsKeyId
        description: The AWS Key Management Service (KMS) key ID of the encryption
          key that you want to            use to encrypt data in the cluster that
          you restore from a shared snapshot
        type: string
      - in: query
        name: NodeType
        description: The node type that the restored cluster will be provisioned with
        type: string
      - in: query
        name: OwnerAccount
        description: The AWS customer account used to create or copy the snapshot
        type: string
      - in: query
        name: Port
        description: The port number on which the cluster accepts connections
        type: string
      - in: query
        name: PreferredMaintenanceWindow
        description: The weekly time range (in UTC) during which automated cluster
          maintenance can            occur
        type: string
      - in: query
        name: PubliclyAccessible
        description: If true, the cluster can be accessed from a public network
        type: string
      - in: query
        name: SnapshotClusterIdentifier
        description: The name of the cluster the source snapshot was created from
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The name of the snapshot from which to create the new cluster
        type: string
      - in: query
        name: VpcSecurityGroupIds.VpcSecurityGroupId.N
        description: A list of Virtual Private Cloud (VPC) security groups to be associated
          with the            cluster
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