{
  "info": {
    "name": "Amazon Redshift API Describe Resize",
    "_postman_id": "ea663ec6-c60d-4d7f-bb08-dbaf94affa5e",
    "description": "Returns information about the last resize operation for the specified cluster.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cluster Security Group",
      "item": [
        {
          "id": "5df385c7-df3c-4c77-8da0-3027b366d4c7",
          "name": "authorizeClusterSecurityGroupIngress",
          "request": {
            "url": "http://example.com/api/?Action=AuthorizeClusterSecurityGroupIngress?CIDRIP=CIDRIP&ClusterSecurityGroupName=ClusterSecurityGroupName&EC2SecurityGroupName=EC2SecurityGroupName&EC2SecurityGroupOwnerId=EC2SecurityGroupOwnerId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds an inbound (ingress) rule to an Amazon Redshift security group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9bc4f934-b7be-433e-8222-e50eb5d717c4"
            }
          ]
        },
        {
          "id": "78b83c55-23b8-4259-ad05-845f81bf5594",
          "name": "createClusterSecurityGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateClusterSecurityGroup?ClusterSecurityGroupName=ClusterSecurityGroupName&Description=Description&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Amazon Redshift security group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "882fee05-c608-46a5-bbb7-a34454e41af0"
            }
          ]
        },
        {
          "id": "469516f7-5685-4612-9b01-adfb056c9afa",
          "name": "deleteClusterSecurityGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteClusterSecurityGroup?ClusterSecurityGroupName=ClusterSecurityGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an Amazon Redshift security group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3596e61d-e891-425d-ad61-d70e9d3ffcc2"
            }
          ]
        },
        {
          "id": "3df73230-b44d-4911-9092-e979bfa8d32b",
          "name": "describeClusterSecurityGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeClusterSecurityGroups?ClusterSecurityGroupName=ClusterSecurityGroupName&Marker=Marker&MaxRecords=MaxRecords&TagKeys.TagKey.N=TagKeys.TagKey.N&TagValues.TagValue.N=TagValues.TagValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about Amazon Redshift security groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "edf6b6b2-dec0-44c7-ad22-31450b2d80f7"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "5a70d589-b41f-4192-bfb5-441991b4333a",
          "name": "authorizeSnapshotAccess",
          "request": {
            "url": "http://example.com/api/?Action=AuthorizeSnapshotAccess?AccountWithRestoreAccess=AccountWithRestoreAccess&SnapshotClusterIdentifier=SnapshotClusterIdentifier&SnapshotIdentifier=SnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Authorizes the specified AWS customer account to restore the specified\n            snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52f38a17-bd94-4040-9b1a-22bd78f2a932"
            }
          ]
        },
        {
          "id": "02ce2278-99a6-46ad-9d2d-5a39abe409de",
          "name": "copyClusterSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CopyClusterSnapshot?SourceSnapshotClusterIdentifier=SourceSnapshotClusterIdentifier&SourceSnapshotIdentifier=SourceSnapshotIdentifier&TargetSnapshotIdentifier=TargetSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified automated cluster snapshot to a new manual cluster snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66d9c435-ade1-43de-82b9-17447c8b5f99"
            }
          ]
        },
        {
          "id": "f2bb37c4-3b91-4ac0-be1f-dbc9520a25f3",
          "name": "createClusterSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateClusterSnapshot?ClusterIdentifier=ClusterIdentifier&SnapshotIdentifier=SnapshotIdentifier&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a manual snapshot of the specified cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34ecdaae-d9e0-4bb8-952e-fba1856db22b"
            }
          ]
        },
        {
          "id": "f5b9e793-f486-4f7c-beba-62b436b63afe",
          "name": "createSnapshotCopyGrant",
          "request": {
            "url": "http://example.com/api/?Action=CreateSnapshotCopyGrant?KmsKeyId=KmsKeyId&SnapshotCopyGrantName=SnapshotCopyGrantName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot copy grant that permits Amazon Redshift to use a customer master key\n            (CMK) from AWS Key Management Service (AWS KMS) to encrypt copied snapshots in a\n            destination region."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15e04db6-84ac-4ec5-b3ab-7ab1ce00fee2"
            }
          ]
        },
        {
          "id": "f6313728-c91b-45fc-a9a8-f53077685d32",
          "name": "deleteClusterSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteClusterSnapshot?SnapshotClusterIdentifier=SnapshotClusterIdentifier&SnapshotIdentifier=SnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified manual snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c29d866-5256-4b86-8468-accdd7d1e75c"
            }
          ]
        },
        {
          "id": "d5f402ba-eb7c-43ab-9b26-44610e07d6ec",
          "name": "deleteSnapshotCopyGrant",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSnapshotCopyGrant?SnapshotCopyGrantName=SnapshotCopyGrantName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified snapshot copy grant."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30f01622-b640-4c39-b0dc-30a408a45a4b"
            }
          ]
        },
        {
          "id": "85c9ff51-2bcc-4e1d-9a76-b1bb250e2f0d",
          "name": "describeClusterSnapshots",
          "request": {
            "url": "http://example.com/api/?Action=DescribeClusterSnapshots?ClusterIdentifier=ClusterIdentifier&EndTime=EndTime&Marker=Marker&MaxRecords=MaxRecords&OwnerAccount=OwnerAccount&SnapshotIdentifier=SnapshotIdentifier&SnapshotType=SnapshotType&StartTime=StartTime&TagKeys.TagKey.N=TagKeys.TagKey.N&TagValues.TagValue.N=TagValues.TagValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns one or more snapshot objects, which contain metadata about your cluster\n            snapshots."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7393f5aa-41ac-4526-9eb8-d98c80a8d67c"
            }
          ]
        }
      ]
    },
    {
      "name": "Clusters",
      "item": [
        {
          "id": "a3332163-09b4-4d77-bd53-c5e19bbece57",
          "name": "createCluster",
          "request": {
            "url": "http://example.com/api/?Action=CreateCluster?AdditionalInfo=AdditionalInfo&AllowVersionUpgrade=AllowVersionUpgrade&AutomatedSnapshotRetentionPeriod=AutomatedSnapshotRetentionPeriod&AvailabilityZone=AvailabilityZone&ClusterIdentifier=ClusterIdentifier&ClusterParameterGroupName=ClusterParameterGroupName&ClusterSecurityGroups.ClusterSecurityGroupName.N=ClusterSecurityGroups.ClusterSecurityGroupName.N&ClusterSubnetGroupName=ClusterSubnetGroupName&ClusterType=ClusterType&ClusterVersion=ClusterVersion&DBName=DBName&ElasticIp=ElasticIp&Encrypted=Encrypted&EnhancedVpcRouting=EnhancedVpcRouting&HsmClientCertificateIdentifier=HsmClientCertificateIdentifier&HsmConfigurationIdentifier=HsmConfigurationIdentifier&IamRoles.IamRoleArn.N=IamRoles.IamRoleArn.N&KmsKeyId=KmsKeyId&MasterUsername=MasterUsername&MasterUserPassword=MasterUserPassword&NodeType=NodeType&NumberOfNodes=NumberOfNodes&Port=Port&PreferredMaintenanceWindow=PreferredMaintenanceWindow&PubliclyAccessible=PubliclyAccessible&Tags.Tag.N=Tags.Tag.N&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2a7c68f-b574-46c9-8039-74d85b0b3ab0"
            }
          ]
        },
        {
          "id": "66e4d41b-6814-438e-a923-9ed42f484336",
          "name": "deleteCluster",
          "request": {
            "url": "http://example.com/api/?Action=DeleteCluster?ClusterIdentifier=ClusterIdentifier&FinalClusterSnapshotIdentifier=FinalClusterSnapshotIdentifier&SkipFinalClusterSnapshot=SkipFinalClusterSnapshot",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a previously provisioned cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3561c3e-e6e4-4a3a-b34e-6a926c2daebc"
            }
          ]
        },
        {
          "id": "3506e3a5-c894-4acb-8f08-50567ab51dd2",
          "name": "describeClusters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeClusters?ClusterIdentifier=ClusterIdentifier&Marker=Marker&MaxRecords=MaxRecords&TagKeys.TagKey.N=TagKeys.TagKey.N&TagValues.TagValue.N=TagValues.TagValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns properties of provisioned clusters including general cluster properties,\n            cluster database properties, maintenance and backup properties, and security and access\n            properties."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ce5a94b-4453-415d-9a5a-33e88791149a"
            }
          ]
        },
        {
          "id": "dfb18016-a727-4c4e-b858-237db58c7c0c",
          "name": "describeClusterVersions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeClusterVersions?ClusterParameterGroupFamily=ClusterParameterGroupFamily&ClusterVersion=ClusterVersion&Marker=Marker&MaxRecords=MaxRecords",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns descriptions of the available Amazon Redshift cluster versions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c01428a8-4168-4952-9d00-7eb64d8cb216"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameter Groups",
      "item": [
        {
          "id": "91c00a21-37ce-4561-a955-5fd68c025fec",
          "name": "createClusterParameterGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateClusterParameterGroup?Description=Description&ParameterGroupFamily=ParameterGroupFamily&ParameterGroupName=ParameterGroupName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an Amazon Redshift parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83cdd3c1-e94e-4256-b328-a0bed6f2cf1e"
            }
          ]
        },
        {
          "id": "bf300445-a6f6-40ac-a0fd-36da22eaa6ac",
          "name": "deleteClusterParameterGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteClusterParameterGroup?ParameterGroupName=ParameterGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified Amazon Redshift parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "546745e2-17f6-4989-942a-438b3e01b548"
            }
          ]
        },
        {
          "id": "35241680-17e9-4434-85fe-ad6256267753",
          "name": "describeClusterParameterGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeClusterParameterGroups?Marker=Marker&MaxRecords=MaxRecords&ParameterGroupName=ParameterGroupName&TagKeys.TagKey.N=TagKeys.TagKey.N&TagValues.TagValue.N=TagValues.TagValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of Amazon Redshift parameter groups, including parameter groups you\n            created and the default parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e60825c-767e-4700-9e05-73afe24a3a12"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Subnet Groups",
      "item": [
        {
          "id": "b856bb01-0a0a-43a9-8b1f-16ab227336ad",
          "name": "createClusterSubnetGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateClusterSubnetGroup?ClusterSubnetGroupName=ClusterSubnetGroupName&Description=Description&SubnetIds.SubnetIdentifier.N=SubnetIds.SubnetIdentifier.N&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Amazon Redshift subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07542940-ea4b-4f02-9dac-3c1bfd91acc1"
            }
          ]
        },
        {
          "id": "df19dd10-434a-4fba-9080-e44b7b2ae518",
          "name": "deleteClusterSubnetGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteClusterSubnetGroup?ClusterSubnetGroupName=ClusterSubnetGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified cluster subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c7c12bc-981e-4505-a196-61f5dabd5ad2"
            }
          ]
        },
        {
          "id": "103ca7fd-29d0-42e4-8446-049127610a3e",
          "name": "describeClusterSubnetGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeClusterSubnetGroups?ClusterSubnetGroupName=ClusterSubnetGroupName&Marker=Marker&MaxRecords=MaxRecords&TagKeys.TagKey.N=TagKeys.TagKey.N&TagValues.TagValue.N=TagValues.TagValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns one or more cluster subnet group objects, which contain metadata about your\n            cluster subnet groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5964717-d16e-4a6d-8e5a-e614e424bb62"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "36e45519-379a-4b89-a64c-80d243ea7943",
          "name": "createEventSubscription",
          "request": {
            "url": "http://example.com/api/?Action=CreateEventSubscription?Enabled=Enabled&EventCategories.EventCategory.N=EventCategories.EventCategory.N&Severity=Severity&SnsTopicArn=SnsTopicArn&SourceIds.SourceId.N=SourceIds.SourceId.N&SourceType=SourceType&SubscriptionName=SubscriptionName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an Amazon Redshift event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "208f3e89-e0e0-42d5-bdc1-4e81862112bf"
            }
          ]
        },
        {
          "id": "c6827f56-6191-4bf4-b7e4-e62e9f7b4ec2",
          "name": "deleteEventSubscription",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEventSubscription?SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an Amazon Redshift event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "872f2303-29b3-4238-b040-4b17d235badf"
            }
          ]
        },
        {
          "id": "a6cca441-a3d9-4158-928a-ae389922d90d",
          "name": "describeEventSubscriptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEventSubscriptions?Marker=Marker&MaxRecords=MaxRecords&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists descriptions of all the Amazon Redshift event notifications subscription for a\n            customer account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12babcf9-b4e6-4afa-8689-b3fd7581dfb7"
            }
          ]
        }
      ]
    },
    {
      "name": "HSM Client Certificates",
      "item": [
        {
          "id": "d97c48c7-f724-4d38-a827-f90f6cebb7de",
          "name": "createHsmClientCertificate",
          "request": {
            "url": "http://example.com/api/?Action=CreateHsmClientCertificate?HsmClientCertificateIdentifier=HsmClientCertificateIdentifier&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an HSM client certificate that an Amazon Redshift cluster will use to connect to\n            the client's HSM in order to store and retrieve the keys used to encrypt the cluster\n            databases."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "266c5d1f-c7c3-48e2-b935-053e0045dcc5"
            }
          ]
        },
        {
          "id": "6daac87b-5b93-464c-968f-ffba6f8ec1ec",
          "name": "deleteHsmClientCertificate",
          "request": {
            "url": "http://example.com/api/?Action=DeleteHsmClientCertificate?HsmClientCertificateIdentifier=HsmClientCertificateIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified HSM client certificate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5967765-a394-48c2-b120-e55209e52151"
            }
          ]
        },
        {
          "id": "66f60a4c-64fe-43b7-bc28-4bf6b2fdc7b3",
          "name": "describeHsmClientCertificates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeHsmClientCertificates?HsmClientCertificateIdentifier=HsmClientCertificateIdentifier&Marker=Marker&MaxRecords=MaxRecords&TagKeys.TagKey.N=TagKeys.TagKey.N&TagValues.TagValue.N=TagValues.TagValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the specified HSM client certificate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e392bddc-ccf7-4db7-84d6-ec6f2285d10c"
            }
          ]
        }
      ]
    },
    {
      "name": "HSM Configurations",
      "item": [
        {
          "id": "dccefb61-3549-4436-90f1-d28d54de3cf2",
          "name": "createHsmConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=CreateHsmConfiguration?Description=Description&HsmConfigurationIdentifier=HsmConfigurationIdentifier&HsmIpAddress=HsmIpAddress&HsmPartitionName=HsmPartitionName&HsmPartitionPassword=HsmPartitionPassword&HsmServerPublicCertificate=HsmServerPublicCertificate&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an HSM configuration that contains the information required by an Amazon Redshift\n            cluster to store and use database encryption keys in a Hardware Security Module (HSM)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "331acd7d-0f5d-42aa-aaad-da237c186785"
            }
          ]
        },
        {
          "id": "081372ae-2345-40c3-bacc-c32896c68834",
          "name": "deleteHsmConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=DeleteHsmConfiguration?HsmConfigurationIdentifier=HsmConfigurationIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Amazon Redshift HSM configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c88e007-8c66-46ff-8c49-9f3ffa588540"
            }
          ]
        },
        {
          "id": "e7497c75-e056-4198-a08f-fd01fea87a76",
          "name": "describeHsmConfigurations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeHsmConfigurations?HsmConfigurationIdentifier=HsmConfigurationIdentifier&Marker=Marker&MaxRecords=MaxRecords&TagKeys.TagKey.N=TagKeys.TagKey.N&TagValues.TagValue.N=TagValues.TagValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the specified Amazon Redshift HSM configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1a3f950-be7e-479f-8c14-cf0ffcf5b94a"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "f6788d65-1e4e-41cd-acb2-7365ad3b23ab",
          "name": "createTags",
          "request": {
            "url": "http://example.com/api/?Action=CreateTags?ResourceName=ResourceName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds one or more tags to a specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd198dfb-bbd9-4a44-8278-36911b9d9ba7"
            }
          ]
        },
        {
          "id": "280f2df0-9b80-4b47-ace1-48875509a678",
          "name": "deleteTags",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTags?ResourceName=ResourceName&TagKeys.TagKey.N=TagKeys.TagKey.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a tag or tags from a resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bfed21c-9b8e-4e0e-b2a9-67fda74e2875"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameters",
      "item": [
        {
          "id": "0d031224-53a5-4ca8-9a6d-715628b9cadb",
          "name": "describeClusterParameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeClusterParameters?Marker=Marker&MaxRecords=MaxRecords&ParameterGroupName=ParameterGroupName&Source=Source",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a detailed list of parameters contained within the specified Amazon Redshift\n            parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6beb1e38-79c8-4c35-8686-c0e325d99f58"
            }
          ]
        },
        {
          "id": "3fabbc0a-2acc-4f10-887f-1bd7ca1a9868",
          "name": "describeDefaultClusterParameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDefaultClusterParameters?Marker=Marker&MaxRecords=MaxRecords&ParameterGroupFamily=ParameterGroupFamily",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of parameter settings for the specified parameter group\n            family."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a35dd952-d752-4a5e-80b8-8c197e78347a"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Categories",
      "item": [
        {
          "id": "69aeac31-7dc1-4ffb-87c8-2a80a2f15a15",
          "name": "describeEventCategories",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEventCategories?SourceType=SourceType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Displays a list of event categories for all event source types, or for a specified\n            source type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63b03825-a76f-45b3-b757-e8a1d434d02b"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "37d06922-fa1b-404e-9441-2d2723bb18d9",
          "name": "describeEvents",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEvents?Duration=Duration&EndTime=EndTime&Marker=Marker&MaxRecords=MaxRecords&SourceIdentifier=SourceIdentifier&SourceType=SourceType&StartTime=StartTime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns events related to clusters, security groups, snapshots, and parameter\n            groups for the past 14 days."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5faca4d6-2076-4811-ba27-5c75ae038148"
            }
          ]
        }
      ]
    },
    {
      "name": "Logging",
      "item": [
        {
          "id": "4c884b29-7a29-4443-b78a-fc7fde5f22a7",
          "name": "describeLoggingStatus",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLoggingStatus?ClusterIdentifier=ClusterIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes whether information, such as queries and connection attempts, is being\n            logged for the specified Amazon Redshift cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c0e996c-8844-49fc-b345-3bd208e3baa2"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Options",
      "item": [
        {
          "id": "d41d9abf-e0a9-4c92-bdd8-0e2483736a43",
          "name": "describeOrderableClusterOptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeOrderableClusterOptions?ClusterVersion=ClusterVersion&Marker=Marker&MaxRecords=MaxRecords&NodeType=NodeType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of orderable cluster options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29cd9a4a-e20c-4460-8ed9-d9d08d1b3eec"
            }
          ]
        }
      ]
    },
    {
      "name": "Reserved Nodes",
      "item": [
        {
          "id": "48b4986f-b323-4ec7-831a-18be1ba72a32",
          "name": "describeReservedNodeOfferings",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReservedNodeOfferings?Marker=Marker&MaxRecords=MaxRecords&ReservedNodeOfferingId=ReservedNodeOfferingId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the available reserved node offerings by Amazon Redshift with their\n            descriptions including the node type, the fixed and recurring costs of reserving the\n            node and duration the node will be reserved for you."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97de82ca-2e01-41c4-a073-2f5c26b24586"
            }
          ]
        },
        {
          "id": "ba5113d8-881c-4ab6-83c0-c886d4105e5d",
          "name": "describeReservedNodes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeReservedNodes?Marker=Marker&MaxRecords=MaxRecords&ReservedNodeId=ReservedNodeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the descriptions of the reserved nodes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1090e88a-b548-40c8-be9b-bc726d79de4d"
            }
          ]
        }
      ]
    },
    {
      "name": "Resize",
      "item": [
        {
          "id": "9bb13a4e-d63f-4289-a919-d561e292da4a",
          "name": "describeResize",
          "request": {
            "url": "http://example.com/api/?Action=DescribeResize?ClusterIdentifier=ClusterIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the last resize operation for the specified cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7fbc0c37-d59a-4dba-86aa-30be020802d5"
            }
          ]
        }
      ]
    }
  ]
}