---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Describe Snapshot Copy Grants
  version: 1.0.0
  description: |-
    Returns a list of snapshot copy grants owned by the AWS account in the destination
                region.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AuthorizeClusterSecurityGroupIngress:
    get:
      summary: Authorize Cluster Security Group Ingress
      description: Adds an inbound (ingress) rule to an Amazon Redshift security group.
      operationId: authorizeClusterSecurityGroupIngress
      x-api-path-slug: actionauthorizeclustersecuritygroupingress-get
      parameters:
      - in: query
        name: CIDRIP
        description: The IP range to be added the Amazon Redshift security group
        type: string
      - in: query
        name: ClusterSecurityGroupName
        description: The name of the security group to which the ingress rule is added
        type: string
      - in: query
        name: EC2SecurityGroupName
        description: The EC2 security group to be added the Amazon Redshift security
          group
        type: string
      - in: query
        name: EC2SecurityGroupOwnerId
        description: The AWS account number of the owner of the security group specified
          by the                EC2SecurityGroupName parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=AuthorizeSnapshotAccess:
    get:
      summary: Authorize Snapshot Access
      description: |-
        Authorizes the specified AWS customer account to restore the specified
                    snapshot.
      operationId: authorizeSnapshotAccess
      x-api-path-slug: actionauthorizesnapshotaccess-get
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
      - Snapshots
  /?Action=CopyClusterSnapshot:
    get:
      summary: Copy Cluster Snapshot
      description: Copies the specified automated cluster snapshot to a new manual
        cluster snapshot.
      operationId: copyClusterSnapshot
      x-api-path-slug: actioncopyclustersnapshot-get
      parameters:
      - in: query
        name: SourceSnapshotClusterIdentifier
        description: The identifier of the cluster the source snapshot was created
          from
        type: string
      - in: query
        name: SourceSnapshotIdentifier
        description: The identifier for the source snapshot
        type: string
      - in: query
        name: TargetSnapshotIdentifier
        description: The identifier given to the new manual snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CreateCluster:
    get:
      summary: Create Cluster
      description: Creates a new cluster.
      operationId: createCluster
      x-api-path-slug: actioncreatecluster-get
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
        description: The EC2 Availability Zone (AZ) in which you want Amazon Redshift
          to provision the            cluster
        type: string
      - in: query
        name: ClusterIdentifier
        description: A unique identifier for the cluster
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
        description: The name of a cluster subnet group to be associated with this
          cluster
        type: string
      - in: query
        name: ClusterType
        description: The type of the cluster
        type: string
      - in: query
        name: ClusterVersion
        description: The version of the Amazon Redshift engine software that you want
          to deploy on the            cluster
        type: string
      - in: query
        name: DBName
        description: The name of the first database to be created when the cluster
          is created
        type: string
      - in: query
        name: ElasticIp
        description: The Elastic IP (EIP) address for the cluster
        type: string
      - in: query
        name: Encrypted
        description: If true, the data in the cluster is encrypted at rest
        type: string
      - in: query
        name: EnhancedVpcRouting
        description: An option that specifies whether to create the cluster with enhanced
          VPC routing            enabled
        type: string
      - in: query
        name: HsmClientCertificateIdentifier
        description: Specifies the name of the HSM client certificate the Amazon Redshift
          cluster uses to           retrieve the data encryption keys stored in an
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
          key that you want to            use to encrypt data in the cluster
        type: string
      - in: query
        name: MasterUsername
        description: The user name associated with the master user account for the
          cluster that is being            created
        type: string
      - in: query
        name: MasterUserPassword
        description: The password associated with the master user account for the
          cluster that is being            created
        type: string
      - in: query
        name: NodeType
        description: The node type to be provisioned for the cluster
        type: string
      - in: query
        name: NumberOfNodes
        description: The number of compute nodes in the cluster
        type: string
      - in: query
        name: Port
        description: The port number on which the cluster accepts incoming connections
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
        name: Tags.Tag.N
        description: A list of tag instances
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
      - Clusters
  /?Action=CreateClusterParameterGroup:
    get:
      summary: Create Cluster Parameter Group
      description: Creates an Amazon Redshift parameter group.
      operationId: createClusterParameterGroup
      x-api-path-slug: actioncreateclusterparametergroup-get
      parameters:
      - in: query
        name: Description
        description: A description of the parameter group
        type: string
      - in: query
        name: ParameterGroupFamily
        description: The Amazon Redshift engine version to which the cluster parameter
          group applies
        type: string
      - in: query
        name: ParameterGroupName
        description: The name of the cluster parameter group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=CreateClusterSecurityGroup:
    get:
      summary: Create Cluster Security Group
      description: Creates a new Amazon Redshift security group.
      operationId: createClusterSecurityGroup
      x-api-path-slug: actioncreateclustersecuritygroup-get
      parameters:
      - in: query
        name: ClusterSecurityGroupName
        description: The name for the security group
        type: string
      - in: query
        name: Description
        description: A description for the security group
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=CreateClusterSnapshot:
    get:
      summary: Create Cluster Snapshot
      description: Creates a manual snapshot of the specified cluster.
      operationId: createClusterSnapshot
      x-api-path-slug: actioncreateclustersnapshot-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The cluster identifier for which you want a snapshot
        type: string
      - in: query
        name: SnapshotIdentifier
        description: A unique identifier for the snapshot that you are requesting
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CreateClusterSubnetGroup:
    get:
      summary: Create Cluster Subnet Group
      description: Creates a new Amazon Redshift subnet group.
      operationId: createClusterSubnetGroup
      x-api-path-slug: actioncreateclustersubnetgroup-get
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name for the subnet group
        type: string
      - in: query
        name: Description
        description: A description for the subnet group
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: An array of VPC subnet IDs
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Subnet Groups
  /?Action=CreateEventSubscription:
    get:
      summary: Create Event Subscription
      description: Creates an Amazon Redshift event notification subscription.
      operationId: createEventSubscription
      x-api-path-slug: actioncreateeventsubscription-get
      parameters:
      - in: query
        name: Enabled
        description: A Boolean value; set to true to activate the subscription, set
          to                false to create the subscription but not active it
        type: string
      - in: query
        name: EventCategories.EventCategory.N
        description: Specifies the Amazon Redshift event categories to be published
          by the event notification            subscription
        type: string
      - in: query
        name: Severity
        description: Specifies the Amazon Redshift event severity to be published
          by the event notification            subscription
        type: string
      - in: query
        name: SnsTopicArn
        description: The Amazon Resource Name (ARN) of the Amazon SNS topic used to
          transmit the event            notifications
        type: string
      - in: query
        name: SourceIds.SourceId.N
        description: A list of one or more identifiers of Amazon Redshift source objects
        type: string
      - in: query
        name: SourceType
        description: The type of source that will be generating the events
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the event subscription to be created
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=CreateHsmClientCertificate:
    get:
      summary: Create Hsm Client Certificate
      description: |-
        Creates an HSM client certificate that an Amazon Redshift cluster will use to connect to
                    the client's HSM in order to store and retrieve the keys used to encrypt the cluster
                    databases.
      operationId: createHsmClientCertificate
      x-api-path-slug: actioncreatehsmclientcertificate-get
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
      - HSM Client Certificates
  /?Action=CreateHsmConfiguration:
    get:
      summary: Create Hsm Configuration
      description: |-
        Creates an HSM configuration that contains the information required by an Amazon Redshift
                    cluster to store and use database encryption keys in a Hardware Security Module (HSM).
      operationId: createHsmConfiguration
      x-api-path-slug: actioncreatehsmconfiguration-get
      parameters:
      - in: query
        name: Description
        description: A text description of the HSM configuration to be created
        type: string
      - in: query
        name: HsmConfigurationIdentifier
        description: The identifier to be assigned to the new Amazon Redshift HSM
          configuration
        type: string
      - in: query
        name: HsmIpAddress
        description: The IP address that the Amazon Redshift cluster must use to access
          the HSM
        type: string
      - in: query
        name: HsmPartitionName
        description: The name of the partition in the HSM where the Amazon Redshift
          clusters will store their            database encryption keys
        type: string
      - in: query
        name: HsmPartitionPassword
        description: The password required to access the HSM partition
        type: string
      - in: query
        name: HsmServerPublicCertificate
        description: The HSMs public certificate file
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Configurations
  /?Action=CreateSnapshotCopyGrant:
    get:
      summary: Create Snapshot Copy Grant
      description: |-
        Creates a snapshot copy grant that permits Amazon Redshift to use a customer master key
                    (CMK) from AWS Key Management Service (AWS KMS) to encrypt copied snapshots in a
                    destination region.
      operationId: createSnapshotCopyGrant
      x-api-path-slug: actioncreatesnapshotcopygrant-get
      parameters:
      - in: query
        name: KmsKeyId
        description: The unique identifier of the customer master key (CMK) to which
          to grant Amazon Redshift            permission
        type: string
      - in: query
        name: SnapshotCopyGrantName
        description: The name of the snapshot copy grant
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=CreateTags:
    get:
      summary: Create Tags
      description: Adds one or more tags to a specified resource.
      operationId: createTags
      x-api-path-slug: actioncreatetags-get
      parameters:
      - in: query
        name: ResourceName
        description: The Amazon Resource Name (ARN) to which you want to add the tag
          or tags
        type: string
      - in: query
        name: Tags.Tag.N
        description: One or more name/value pairs to add as tags to the specified
          resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=DeleteCluster:
    get:
      summary: Delete Cluster
      description: Deletes a previously provisioned cluster.
      operationId: deleteCluster
      x-api-path-slug: actiondeletecluster-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The identifier of the cluster to be deleted
        type: string
      - in: query
        name: FinalClusterSnapshotIdentifier
        description: The identifier of the final snapshot that is to be created immediately
          before            deleting the cluster
        type: string
      - in: query
        name: SkipFinalClusterSnapshot
        description: Determines whether a final snapshot of the cluster is created
          before Amazon Redshift            deletes the cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DeleteClusterParameterGroup:
    get:
      summary: Delete Cluster Parameter Group
      description: Deletes a specified Amazon Redshift parameter group.
      operationId: deleteClusterParameterGroup
      x-api-path-slug: actiondeleteclusterparametergroup-get
      parameters:
      - in: query
        name: ParameterGroupName
        description: The name of the parameter group to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=DeleteClusterSecurityGroup:
    get:
      summary: Delete Cluster Security Group
      description: Deletes an Amazon Redshift security group.
      operationId: deleteClusterSecurityGroup
      x-api-path-slug: actiondeleteclustersecuritygroup-get
      parameters:
      - in: query
        name: ClusterSecurityGroupName
        description: The name of the cluster security group to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=DeleteClusterSnapshot:
    get:
      summary: Delete Cluster Snapshot
      description: Deletes the specified manual snapshot.
      operationId: deleteClusterSnapshot
      x-api-path-slug: actiondeleteclustersnapshot-get
      parameters:
      - in: query
        name: SnapshotClusterIdentifier
        description: The unique identifier of the cluster the snapshot was created
          from
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The unique identifier of the manual snapshot to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DeleteClusterSubnetGroup:
    get:
      summary: Delete Cluster Subnet Group
      description: Deletes the specified cluster subnet group.
      operationId: deleteClusterSubnetGroup
      x-api-path-slug: actiondeleteclustersubnetgroup-get
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name of the cluster subnet group name to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Subnet Groups
  /?Action=DeleteEventSubscription:
    get:
      summary: Delete Event Subscription
      description: Deletes an Amazon Redshift event notification subscription.
      operationId: deleteEventSubscription
      x-api-path-slug: actiondeleteeventsubscription-get
      parameters:
      - in: query
        name: SubscriptionName
        description: The name of the Amazon Redshift event notification subscription
          to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=DeleteHsmClientCertificate:
    get:
      summary: Delete Hsm Client Certificate
      description: Deletes the specified HSM client certificate.
      operationId: deleteHsmClientCertificate
      x-api-path-slug: actiondeletehsmclientcertificate-get
      parameters:
      - in: query
        name: HsmClientCertificateIdentifier
        description: The identifier of the HSM client certificate to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Client Certificates
  /?Action=DeleteHsmConfiguration:
    get:
      summary: Delete Hsm Configuration
      description: Deletes the specified Amazon Redshift HSM configuration.
      operationId: deleteHsmConfiguration
      x-api-path-slug: actiondeletehsmconfiguration-get
      parameters:
      - in: query
        name: HsmConfigurationIdentifier
        description: The identifier of the Amazon Redshift HSM configuration to be
          deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Configurations
  /?Action=DeleteSnapshotCopyGrant:
    get:
      summary: Delete Snapshot Copy Grant
      description: Deletes the specified snapshot copy grant.
      operationId: deleteSnapshotCopyGrant
      x-api-path-slug: actiondeletesnapshotcopygrant-get
      parameters:
      - in: query
        name: SnapshotCopyGrantName
        description: The name of the snapshot copy grant to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DeleteTags:
    get:
      summary: Delete Tags
      description: Deletes a tag or tags from a resource.
      operationId: deleteTags
      x-api-path-slug: actiondeletetags-get
      parameters:
      - in: query
        name: ResourceName
        description: The Amazon Resource Name (ARN) from which you want to remove
          the tag or tags
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: The tag key that you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tags
  /?Action=DescribeClusterParameterGroups:
    get:
      summary: Describe Cluster Parameter Groups
      description: |-
        Returns a list of Amazon Redshift parameter groups, including parameter groups you
                    created and the default parameter group.
      operationId: describeClusterParameterGroups
      x-api-path-slug: actiondescribeclusterparametergroups-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ParameterGroupName
        description: The name of a specific parameter group for which to return details
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          parameter            groups that are associated with the specified key or
          keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster parameter            groups that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=DescribeClusterParameters:
    get:
      summary: Describe Cluster Parameters
      description: |-
        Returns a detailed list of parameters contained within the specified Amazon Redshift
                    parameter group.
      operationId: describeClusterParameters
      x-api-path-slug: actiondescribeclusterparameters-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ParameterGroupName
        description: The name of a cluster parameter group for which to return details
        type: string
      - in: query
        name: Source
        description: The parameter types to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameters
  /?Action=DescribeClusters:
    get:
      summary: Describe Clusters
      description: |-
        Returns properties of provisioned clusters including general cluster properties,
                    cluster database properties, maintenance and backup properties, and security and access
                    properties.
      operationId: describeClusters
      x-api-path-slug: actiondescribeclusters-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of a cluster whose properties you are requesting
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching clusters
          that are            associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          clusters that are            associated with the specified tag value or
          values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DescribeClusterSecurityGroups:
    get:
      summary: Describe Cluster Security Groups
      description: Returns information about Amazon Redshift security groups.
      operationId: describeClusterSecurityGroups
      x-api-path-slug: actiondescribeclustersecuritygroups-get
      parameters:
      - in: query
        name: ClusterSecurityGroupName
        description: The name of a cluster security group for which you are requesting
          details
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          security groups            that are associated with the specified key or
          keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster security            groups that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Security Group
  /?Action=DescribeClusterSnapshots:
    get:
      summary: Describe Cluster Snapshots
      description: |-
        Returns one or more snapshot objects, which contain metadata about your cluster
                    snapshots.
      operationId: describeClusterSnapshots
      x-api-path-slug: actiondescribeclustersnapshots-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The identifier of the cluster for which information about snapshots
          is            requested
        type: string
      - in: query
        name: EndTime
        description: A time value that requests only snapshots created at or before
          the specified time
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: OwnerAccount
        description: The AWS customer account used to create or copy the snapshot
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The snapshot identifier of the snapshot about which to return            information
        type: string
      - in: query
        name: SnapshotType
        description: The type of snapshots for which you are requesting information
        type: string
      - in: query
        name: StartTime
        description: A value that requests only snapshots created at or after the
          specified time
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          snapshots that            are associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster snapshots            that are associated with the specified tag
          value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DescribeClusterSubnetGroups:
    get:
      summary: Describe Cluster Subnet Groups
      description: |-
        Returns one or more cluster subnet group objects, which contain metadata about your
                    cluster subnet groups.
      operationId: describeClusterSubnetGroups
      x-api-path-slug: actiondescribeclustersubnetgroups-get
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name of the cluster subnet group for which information is
          requested
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching cluster
          subnet groups            that are associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          cluster subnet            groups that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Subnet Groups
  /?Action=DescribeClusterVersions:
    get:
      summary: Describe Cluster Versions
      description: Returns descriptions of the available Amazon Redshift cluster versions.
      operationId: describeClusterVersions
      x-api-path-slug: actiondescribeclusterversions-get
      parameters:
      - in: query
        name: ClusterParameterGroupFamily
        description: The name of a specific cluster parameter group family to return
          details            for
        type: string
      - in: query
        name: ClusterVersion
        description: The specific cluster version to return
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /?Action=DescribeDefaultClusterParameters:
    get:
      summary: Describe Default Cluster Parameters
      description: |-
        Returns a list of parameter settings for the specified parameter group
                    family.
      operationId: describeDefaultClusterParameters
      x-api-path-slug: actiondescribedefaultclusterparameters-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ParameterGroupFamily
        description: The name of the cluster parameter group family
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameters
  /?Action=DescribeEventCategories:
    get:
      summary: Describe Event Categories
      description: |-
        Displays a list of event categories for all event source types, or for a specified
                    source type.
      operationId: describeEventCategories
      x-api-path-slug: actiondescribeeventcategories-get
      parameters:
      - in: query
        name: SourceType
        description: The source type, such as cluster or parameter group, to which
          the described event            categories apply
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Categories
  /?Action=DescribeEvents:
    get:
      summary: Describe Events
      description: |-
        Returns events related to clusters, security groups, snapshots, and parameter
                    groups for the past 14 days.
      operationId: describeEvents
      x-api-path-slug: actiondescribeevents-get
      parameters:
      - in: query
        name: Duration
        description: The number of minutes prior to the time of the request for which
          to retrieve            events
        type: string
      - in: query
        name: EndTime
        description: The end of the time interval for which to retrieve events, specified
          in ISO 8601            format
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: SourceIdentifier
        description: The identifier of the event source for which events will be returned
        type: string
      - in: query
        name: SourceType
        description: The event source to retrieve events for
        type: string
      - in: query
        name: StartTime
        description: The beginning of the time interval to retrieve events for, specified
          in ISO 8601            format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
  /?Action=DescribeEventSubscriptions:
    get:
      summary: Describe Event Subscriptions
      description: |-
        Lists descriptions of all the Amazon Redshift event notifications subscription for a
                    customer account.
      operationId: describeEventSubscriptions
      x-api-path-slug: actiondescribeeventsubscriptions-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: SubscriptionName
        description: The name of the Amazon Redshift event notification subscription
          to be            described
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event Subscriptions
  /?Action=DescribeHsmClientCertificates:
    get:
      summary: Describe Hsm Client Certificates
      description: Returns information about the specified HSM client certificate.
      operationId: describeHsmClientCertificates
      x-api-path-slug: actiondescribehsmclientcertificates-get
      parameters:
      - in: query
        name: HsmClientCertificateIdentifier
        description: The identifier of a specific HSM client certificate for which
          you want information
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching HSM
          client certificates            that are associated with the specified key
          or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          HSM client            certificates that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Client Certificates
  /?Action=DescribeHsmConfigurations:
    get:
      summary: Describe Hsm Configurations
      description: Returns information about the specified Amazon Redshift HSM configuration.
      operationId: describeHsmConfigurations
      x-api-path-slug: actiondescribehsmconfigurations-get
      parameters:
      - in: query
        name: HsmConfigurationIdentifier
        description: The identifier of a specific Amazon Redshift HSM configuration
          to be described
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching HSM
          configurations that            are associated with the specified key or
          keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          HSM configurations            that are associated with the specified tag
          value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Configurations
  /?Action=DescribeLoggingStatus:
    get:
      summary: Describe Logging Status
      description: |-
        Describes whether information, such as queries and connection attempts, is being
                    logged for the specified Amazon Redshift cluster.
      operationId: describeLoggingStatus
      x-api-path-slug: actiondescribeloggingstatus-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The identifier of the cluster from which to get the logging status
        type: string
      responses:
        200:
          description: OK
      tags:
      - Logging
  /?Action=DescribeOrderableClusterOptions:
    get:
      summary: Describe Orderable Cluster Options
      description: Returns a list of orderable cluster options.
      operationId: describeOrderableClusterOptions
      x-api-path-slug: actiondescribeorderableclusteroptions-get
      parameters:
      - in: query
        name: ClusterVersion
        description: The version filter value
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: NodeType
        description: The node type filter value
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Options
  /?Action=DescribeReservedNodeOfferings:
    get:
      summary: Describe Reserved Node Offerings
      description: |-
        Returns a list of the available reserved node offerings by Amazon Redshift with their
                    descriptions including the node type, the fixed and recurring costs of reserving the
                    node and duration the node will be reserved for you.
      operationId: describeReservedNodeOfferings
      x-api-path-slug: actiondescribereservednodeofferings-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ReservedNodeOfferingId
        description: The unique identifier for the offering
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Nodes
  /?Action=DescribeReservedNodes:
    get:
      summary: Describe Reserved Nodes
      description: Returns the descriptions of the reserved nodes.
      operationId: describeReservedNodes
      x-api-path-slug: actiondescribereservednodes-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: ReservedNodeId
        description: Identifier for the node reservation
        type: string
      responses:
        200:
          description: OK
      tags:
      - Reserved Nodes
  /?Action=DescribeResize:
    get:
      summary: Describe Resize
      description: Returns information about the last resize operation for the specified
        cluster.
      operationId: describeResize
      x-api-path-slug: actiondescriberesize-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of a cluster whose resize progress you
          are requesting
        type: string
      responses:
        200:
          description: OK
      tags:
      - Resize
  /?Action=DescribeSnapshotCopyGrants:
    get:
      summary: Describe Snapshot Copy Grants
      description: |-
        Returns a list of snapshot copy grants owned by the AWS account in the destination
                    region.
      operationId: describeSnapshotCopyGrants
      x-api-path-slug: actiondescribesnapshotcopygrants-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: SnapshotCopyGrantName
        description: The name of the snapshot copy grant
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching resources
          that are            associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          resources that are            associated with the specified value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
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