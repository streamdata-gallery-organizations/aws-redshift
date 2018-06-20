---
name: AWS Redshift
x-slug: aws-redshift
description: Amazon Redshift is a fast, fully managed, petabyte-scaledata warehousethat
  makes it simple and cost-effective to analyze all your data using your existing
  business intelligence tools. Start small for $0.25 per hour with no commitments
  and scale to petabytes for $1,000 per terabyte per year, less than a tenth the cost
  of traditional solutions. Customers typically see 3x compression, reducing their
  costs to $333 per uncompressed terabyte per year.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
x-kinRank: "10"
x-alexaRank: "0"
tags: AWS Redshift
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/apis.md
specificationVersion: "0.14"
apis:
- name: Amazon Redshift API Authorize Cluster Security Group Ingress
  x-api-slug: amazon-redshift-api
  description: Adds an inbound (ingress) rule to an Amazon Redshift security group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=AuthorizeClusterSecurityGroupIngress
  tags: Cluster Security Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionauthorizeclustersecuritygroupingress-get-openapi.md
- name: Amazon Redshift API Authorize Snapshot Access
  x-api-slug: amazon-redshift-api
  description: |-
    Authorizes the specified AWS customer account to restore the specified
                snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=AuthorizeSnapshotAccess
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionauthorizesnapshotaccess-get-openapi.md
- name: Amazon Redshift API Copy Cluster Snapshot
  x-api-slug: amazon-redshift-api
  description: Copies the specified automated cluster snapshot to a new manual cluster
    snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CopyClusterSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actioncopyclustersnapshot-get-openapi.md
- name: Amazon Redshift API Create Cluster
  x-api-slug: amazon-redshift-api
  description: Creates a new cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CreateCluster
  tags: Clusters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actioncreatecluster-get-openapi.md
- name: Amazon Redshift API Create Cluster Parameter Group
  x-api-slug: amazon-redshift-api
  description: Creates an Amazon Redshift parameter group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CreateClusterParameterGroup
  tags: Cluster Parameter Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actioncreateclusterparametergroup-get-openapi.md
- name: Amazon Redshift API Create Cluster Security Group
  x-api-slug: amazon-redshift-api
  description: Creates a new Amazon Redshift security group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CreateClusterSecurityGroup
  tags: Cluster Security Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actioncreateclustersecuritygroup-get-openapi.md
- name: Amazon Redshift API Create Cluster Snapshot
  x-api-slug: amazon-redshift-api
  description: Creates a manual snapshot of the specified cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CreateClusterSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actioncreateclustersnapshot-get-openapi.md
- name: Amazon Redshift API Create Cluster Subnet Group
  x-api-slug: amazon-redshift-api
  description: Creates a new Amazon Redshift subnet group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CreateClusterSubnetGroup
  tags: Cluster Subnet Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actioncreateclustersubnetgroup-get-openapi.md
- name: Amazon Redshift API Create Event Subscription
  x-api-slug: amazon-redshift-api
  description: Creates an Amazon Redshift event notification subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CreateEventSubscription
  tags: Event Subscriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actioncreateeventsubscription-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actioncreateeventsubscription-get-openapi.md
- name: Amazon Redshift API Create Hsm Client Certificate
  x-api-slug: amazon-redshift-api
  description: |-
    Creates an HSM client certificate that an Amazon Redshift cluster will use to connect to
                the client's HSM in order to store and retrieve the keys used to encrypt the cluster
                databases.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CreateHsmClientCertificate
  tags: HSM Client Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actioncreatehsmclientcertificate-get-openapi.md
- name: Amazon Redshift API Create Hsm Configuration
  x-api-slug: amazon-redshift-api
  description: |-
    Creates an HSM configuration that contains the information required by an Amazon Redshift
                cluster to store and use database encryption keys in a Hardware Security Module (HSM).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CreateHsmConfiguration
  tags: HSM Configurations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actioncreatehsmconfiguration-get-openapi.md
- name: Amazon Redshift API Create Snapshot Copy Grant
  x-api-slug: amazon-redshift-api
  description: |-
    Creates a snapshot copy grant that permits Amazon Redshift to use a customer master key
                (CMK) from AWS Key Management Service (AWS KMS) to encrypt copied snapshots in a
                destination region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CreateSnapshotCopyGrant
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actioncreatesnapshotcopygrant-get-openapi.md
- name: Amazon Redshift API Create Tags
  x-api-slug: amazon-redshift-api
  description: Adds one or more tags to a specified resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=CreateTags
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actioncreatetags-get-openapi.md
- name: Amazon Redshift API Delete Cluster
  x-api-slug: amazon-redshift-api
  description: Deletes a previously provisioned cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DeleteCluster
  tags: Clusters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondeletecluster-get-openapi.md
- name: Amazon Redshift API Delete Cluster Parameter Group
  x-api-slug: amazon-redshift-api
  description: Deletes a specified Amazon Redshift parameter group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DeleteClusterParameterGroup
  tags: Cluster Parameter Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondeleteclusterparametergroup-get-openapi.md
- name: Amazon Redshift API Delete Cluster Security Group
  x-api-slug: amazon-redshift-api
  description: Deletes an Amazon Redshift security group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DeleteClusterSecurityGroup
  tags: Cluster Security Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondeleteclustersecuritygroup-get-openapi.md
- name: Amazon Redshift API Delete Cluster Snapshot
  x-api-slug: amazon-redshift-api
  description: Deletes the specified manual snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DeleteClusterSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondeleteclustersnapshot-get-openapi.md
- name: Amazon Redshift API Delete Cluster Subnet Group
  x-api-slug: amazon-redshift-api
  description: Deletes the specified cluster subnet group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DeleteClusterSubnetGroup
  tags: Cluster Subnet Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondeleteclustersubnetgroup-get-openapi.md
- name: Amazon Redshift API Delete Event Subscription
  x-api-slug: amazon-redshift-api
  description: Deletes an Amazon Redshift event notification subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DeleteEventSubscription
  tags: Event Subscriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondeleteeventsubscription-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondeleteeventsubscription-get-openapi.md
- name: Amazon Redshift API Delete Hsm Client Certificate
  x-api-slug: amazon-redshift-api
  description: Deletes the specified HSM client certificate.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DeleteHsmClientCertificate
  tags: HSM Client Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondeletehsmclientcertificate-get-openapi.md
- name: Amazon Redshift API Delete Hsm Configuration
  x-api-slug: amazon-redshift-api
  description: Deletes the specified Amazon Redshift HSM configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DeleteHsmConfiguration
  tags: HSM Configurations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondeletehsmconfiguration-get-openapi.md
- name: Amazon Redshift API Delete Snapshot Copy Grant
  x-api-slug: amazon-redshift-api
  description: Deletes the specified snapshot copy grant.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DeleteSnapshotCopyGrant
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondeletesnapshotcopygrant-get-openapi.md
- name: Amazon Redshift API Delete Tags
  x-api-slug: amazon-redshift-api
  description: Deletes a tag or tags from a resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DeleteTags
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondeletetags-get-openapi.md
- name: Amazon Redshift API Describe Cluster Parameter Groups
  x-api-slug: amazon-redshift-api
  description: |-
    Returns a list of Amazon Redshift parameter groups, including parameter groups you
                created and the default parameter group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeClusterParameterGroups
  tags: Cluster Parameter Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribeclusterparametergroups-get-openapi.md
- name: Amazon Redshift API Describe Cluster Parameters
  x-api-slug: amazon-redshift-api
  description: |-
    Returns a detailed list of parameters contained within the specified Amazon Redshift
                parameter group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeClusterParameters
  tags: 'Cluster Parameters '
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribeclusterparameters-get-openapi.md
- name: Amazon Redshift API Describe Clusters
  x-api-slug: amazon-redshift-api
  description: |-
    Returns properties of provisioned clusters including general cluster properties,
                cluster database properties, maintenance and backup properties, and security and access
                properties.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeClusters
  tags: Clusters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribeclusters-get-openapi.md
- name: Amazon Redshift API Describe Cluster Security Groups
  x-api-slug: amazon-redshift-api
  description: Returns information about Amazon Redshift security groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeClusterSecurityGroups
  tags: Cluster Security Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribeclustersecuritygroups-get-openapi.md
- name: Amazon Redshift API Describe Cluster Snapshots
  x-api-slug: amazon-redshift-api
  description: |-
    Returns one or more snapshot objects, which contain metadata about your cluster
                snapshots.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeClusterSnapshots
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribeclustersnapshots-get-openapi.md
- name: Amazon Redshift API Describe Cluster Subnet Groups
  x-api-slug: amazon-redshift-api
  description: |-
    Returns one or more cluster subnet group objects, which contain metadata about your
                cluster subnet groups.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeClusterSubnetGroups
  tags: Cluster Subnet Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribeclustersubnetgroups-get-openapi.md
- name: Amazon Redshift API Describe Cluster Versions
  x-api-slug: amazon-redshift-api
  description: Returns descriptions of the available Amazon Redshift cluster versions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeClusterVersions
  tags: Clusters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribeclusterversions-get-openapi.md
- name: Amazon Redshift API Describe Default Cluster Parameters
  x-api-slug: amazon-redshift-api
  description: |-
    Returns a list of parameter settings for the specified parameter group
                family.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeDefaultClusterParameters
  tags: 'Cluster Parameters '
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribedefaultclusterparameters-get-openapi.md
- name: Amazon Redshift API Describe Event Categories
  x-api-slug: amazon-redshift-api
  description: |-
    Displays a list of event categories for all event source types, or for a specified
                source type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeEventCategories
  tags: 'Event Categories '
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribeeventcategories-get-openapi.md
- name: Amazon Redshift API Describe Events
  x-api-slug: amazon-redshift-api
  description: |-
    Returns events related to clusters, security groups, snapshots, and parameter
                groups for the past 14 days.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeEvents
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribeevents-get-openapi.md
- name: Amazon Redshift API Describe Event Subscriptions
  x-api-slug: amazon-redshift-api
  description: |-
    Lists descriptions of all the Amazon Redshift event notifications subscription for a
                customer account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeEventSubscriptions
  tags: Event Subscriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribeeventsubscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribeeventsubscriptions-get-openapi.md
- name: Amazon Redshift API Describe Hsm Client Certificates
  x-api-slug: amazon-redshift-api
  description: Returns information about the specified HSM client certificate.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeHsmClientCertificates
  tags: HSM Client Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribehsmclientcertificates-get-openapi.md
- name: Amazon Redshift API Describe Hsm Configurations
  x-api-slug: amazon-redshift-api
  description: Returns information about the specified Amazon Redshift HSM configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeHsmConfigurations
  tags: HSM Configurations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribehsmconfigurations-get-openapi.md
- name: Amazon Redshift API Describe Logging Status
  x-api-slug: amazon-redshift-api
  description: |-
    Describes whether information, such as queries and connection attempts, is being
                logged for the specified Amazon Redshift cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeLoggingStatus
  tags: Logging
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribeloggingstatus-get-openapi.md
- name: Amazon Redshift API Describe Orderable Cluster Options
  x-api-slug: amazon-redshift-api
  description: Returns a list of orderable cluster options.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeOrderableClusterOptions
  tags: Cluster Options
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribeorderableclusteroptions-get-openapi.md
- name: Amazon Redshift API Describe Reserved Node Offerings
  x-api-slug: amazon-redshift-api
  description: |-
    Returns a list of the available reserved node offerings by Amazon Redshift with their
                descriptions including the node type, the fixed and recurring costs of reserving the
                node and duration the node will be reserved for you.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeReservedNodeOfferings
  tags: 'Reserved Nodes '
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribereservednodeofferings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribereservednodeofferings-get-openapi.md
- name: Amazon Redshift API Describe Reserved Nodes
  x-api-slug: amazon-redshift-api
  description: Returns the descriptions of the reserved nodes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeReservedNodes
  tags: 'Reserved Nodes '
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribereservednodes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribereservednodes-get-openapi.md
- name: Amazon Redshift API Describe Resize
  x-api-slug: amazon-redshift-api
  description: Returns information about the last resize operation for the specified
    cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeResize
  tags: Resize
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescriberesize-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescriberesize-get-openapi.md
- name: Amazon Redshift API Describe Snapshot Copy Grants
  x-api-slug: amazon-redshift-api
  description: |-
    Returns a list of snapshot copy grants owned by the AWS account in the destination
                region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeSnapshotCopyGrants
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribesnapshotcopygrants-get-openapi.md
- name: Amazon Redshift API Describe Table Restore Status
  x-api-slug: amazon-redshift-api
  description: Lists the status of one or more table restore requests made using the.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeTableRestoreStatus
  tags: Tables
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribetablerestorestatus-get-openapi.md
- name: Amazon Redshift API Describe Tags
  x-api-slug: amazon-redshift-api
  description: Returns a list of tags.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DescribeTags
  tags: Tags
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondescribetags-get-openapi.md
- name: Amazon Redshift API Disable Logging
  x-api-slug: amazon-redshift-api
  description: |-
    Stops logging information, such as queries and connection attempts, for the
                specified Amazon Redshift cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DisableLogging
  tags: Logging
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondisablelogging-get-openapi.md
- name: Amazon Redshift API Disable Snapshot Copy
  x-api-slug: amazon-redshift-api
  description: |-
    Disables the automatic copying of snapshots from one region to another region for a
                specified cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=DisableSnapshotCopy
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actiondisablesnapshotcopy-get-openapi.md
- name: Amazon Redshift API Enable Logging
  x-api-slug: amazon-redshift-api
  description: |-
    Starts logging information, such as queries and connection attempts, for the
                specified Amazon Redshift cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=EnableLogging
  tags: Logging
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionenablelogging-get-openapi.md
- name: Amazon Redshift API Enable Snapshot Copy
  x-api-slug: amazon-redshift-api
  description: |-
    Enables the automatic copy of snapshots from one region to another region for a
                specified cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=EnableSnapshotCopy
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionenablesnapshotcopy-get-openapi.md
- name: Amazon Redshift API Modify Cluster
  x-api-slug: amazon-redshift-api
  description: Modifies the settings for a cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=ModifyCluster
  tags: Clusters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionmodifycluster-get-openapi.md
- name: Amazon Redshift API Modify Cluster Iam Roles
  x-api-slug: amazon-redshift-api
  description: |-
    Modifies the list of AWS Identity and Access Management (IAM) roles that can be
                used by the cluster to access other AWS services.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=ModifyClusterIamRoles
  tags: Cluster IAM Roles
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionmodifyclusteriamroles-get-openapi.md
- name: Amazon Redshift API Modify Cluster Parameter Group
  x-api-slug: amazon-redshift-api
  description: Modifies the parameters of a parameter group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=ModifyClusterParameterGroup
  tags: Cluster Parameter Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionmodifyclusterparametergroup-get-openapi.md
- name: Amazon Redshift API Modify Cluster Subnet Group
  x-api-slug: amazon-redshift-api
  description: Modifies a cluster subnet group to include the specified list of VPC
    subnets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=ModifyClusterSubnetGroup
  tags: Cluster Subnet Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionmodifyclustersubnetgroup-get-openapi.md
- name: Amazon Redshift API Modify Event Subscription
  x-api-slug: amazon-redshift-api
  description: Modifies an existing Amazon Redshift event notification subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=ModifyEventSubscription
  tags: Event Subscriptions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionmodifyeventsubscription-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionmodifyeventsubscription-get-openapi.md
- name: Amazon Redshift API Modify Snapshot Copy Retention Period
  x-api-slug: amazon-redshift-api
  description: |-
    Modifies the number of days to retain automated snapshots in the destination region
                after they are copied from the source region.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=ModifySnapshotCopyRetentionPeriod
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionmodifysnapshotcopyretentionperiod-get-openapi.md
- name: Amazon Redshift API Purchase Reserved Node Offering
  x-api-slug: amazon-redshift-api
  description: Allows you to purchase reserved nodes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=PurchaseReservedNodeOffering
  tags: Reserved Nodes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionpurchasereservednodeoffering-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionpurchasereservednodeoffering-get-openapi.md
- name: Amazon Redshift API Reboot Cluster
  x-api-slug: amazon-redshift-api
  description: Reboots a cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=RebootCluster
  tags: Clusters
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionrebootcluster-get-openapi.md
- name: Amazon Redshift API Reset Cluster Parameter Group
  x-api-slug: amazon-redshift-api
  description: |-
    Sets one or more parameters of the specified parameter group to their default
                values and sets the source values of the parameters to "engine-default".
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=ResetClusterParameterGroup
  tags: Cluster Parameter Groups
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionresetclusterparametergroup-get-openapi.md
- name: Amazon Redshift API Restore From Cluster Snapshot
  x-api-slug: amazon-redshift-api
  description: Creates a new cluster from a snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=RestoreFromClusterSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionrestorefromclustersnapshot-get-openapi.md
- name: Amazon Redshift API Restore Table From Cluster Snapshot
  x-api-slug: amazon-redshift-api
  description: Creates a new table from a table in an Amazon Redshift cluster snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=RestoreTableFromClusterSnapshot
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionrestoretablefromclustersnapshot-get-openapi.md
- name: Amazon Redshift API Revoke Cluster Security Group Ingress
  x-api-slug: amazon-redshift-api
  description: |-
    Revokes an ingress rule in an Amazon Redshift security group for a previously authorized
                IP range or Amazon EC2 security group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=RevokeClusterSecurityGroupIngress
  tags: Cluster Security Group
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionrevokeclustersecuritygroupingress-get-openapi.md
- name: Amazon Redshift API Revoke Snapshot Access
  x-api-slug: amazon-redshift-api
  description: |-
    Removes the ability of the specified AWS customer account to restore the specified
                snapshot.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=RevokeSnapshotAccess
  tags: Snapshots
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionrevokesnapshotaccess-get-openapi.md
- name: Amazon Redshift API Rotate Encryption Key
  x-api-slug: amazon-redshift-api
  description: Rotates the encryption keys for a cluster.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: ://///?Action=RotateEncryptionKey
  tags: Encryption Keys
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/actionrotateencryptionkey-get-openapi.md
- name: Amazon Redshift API
  x-api-slug: amazon-redshift-api
  description: Amazon Redshift is a fast, fully managed, petabyte-scaledata warehousethat
    makes it simple and cost-effective to analyze all your data using your existing
    business intelligence tools. Start small for $0.25 per hour with no commitments
    and scale to petabytes for $1,000 per terabyte per year, less than a tenth the
    cost of traditional solutions. Customers typically see 3x compression, reducing
    their costs to $333 per uncompressed terabyte per year.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Database_AmazonRedshift.png
  humanURL: https://aws.amazon.com/redshift/
  baseURL: :///
  tags: AWS Redshift
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/aws-redshift/master/_listings/aws-redshift/openapi.md
x-common:
- type: x-best-practices
  url: https://aws.amazon.com/redshift/developer-resources/#best-practices
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/redshift/index.html
- type: x-customer-success
  url: https://aws.amazon.com/redshift/customer-success/
- type: x-documentation
  url: http://docs.aws.amazon.com/redshift/latest/APIReference/
- type: x-events
  url: https://aws.amazon.com/redshift/events/
- type: x-faq
  url: https://aws.amazon.com/redshift/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/redshift/getting-started/
- type: x-partners
  url: https://aws.amazon.com/redshift/partners/
- type: x-pricing
  url: https://aws.amazon.com/redshift/pricing/
- type: x-website
  url: https://aws.amazon.com/redshift/
- type: x-whats-new
  url: https://aws.amazon.com/redshift/whats-new/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---