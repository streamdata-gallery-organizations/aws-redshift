{
  "info": {
    "name": "Amazon Redshift API Modify Event Subscription",
    "_postman_id": "9373ab6b-fd81-4053-a9a4-323e9785235a",
    "description": "Modifies an existing Amazon Redshift event notification subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cluster Security Group",
      "item": [
        {
          "id": "a4a74f94-57e2-40e2-8a52-7733a2de82d4",
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
              "id": "6924d61f-e0ad-41ce-af88-a19857c3daf1"
            }
          ]
        },
        {
          "id": "4192a013-6b51-42a4-806b-dcc5a831edca",
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
              "id": "57adb814-5e43-4b4a-a936-a0f560b8ef6b"
            }
          ]
        },
        {
          "id": "af1906e9-4929-40b7-a687-587e4fbde369",
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
              "id": "00acbdc0-08be-483d-82f3-d739bb8e38f0"
            }
          ]
        },
        {
          "id": "87b98f50-a264-4aba-bf28-926a72a77676",
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
              "id": "b4a247a4-65ad-4ed8-9dbf-38e237c61bab"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "a59cec2b-7255-48f8-bef0-4953a9a7a43f",
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
              "id": "f203aed7-5d9e-4a68-af64-c9ddad28ea49"
            }
          ]
        },
        {
          "id": "af655514-e2c6-4102-990f-c037338e55ae",
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
              "id": "00cb5733-e86b-4c0e-bd5c-74ac5c63db50"
            }
          ]
        },
        {
          "id": "53152419-bc26-45c5-914e-a199106b7248",
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
              "id": "3d97e062-8f26-432e-bc52-bba2c395f497"
            }
          ]
        },
        {
          "id": "3c4deee3-1b09-4c5b-9810-d72888d87149",
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
              "id": "a48f8bd4-fde6-4038-98b0-2c67acefb395"
            }
          ]
        },
        {
          "id": "5f6648f2-1c11-4001-b40d-663a525cd6e3",
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
              "id": "5ed76bcb-db43-4574-95cf-56b1c53c6986"
            }
          ]
        },
        {
          "id": "477dad55-f5f4-4528-9ed9-f146dddc90be",
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
              "id": "2f846f1c-d429-43aa-b3f6-fc6768cc8ab7"
            }
          ]
        },
        {
          "id": "bfcdb23b-2de7-47f6-8f37-59c8491d5150",
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
              "id": "4087ed13-7d23-4e0a-beec-9960f53bec26"
            }
          ]
        },
        {
          "id": "bda39073-c089-4994-8631-85eaa4f288aa",
          "name": "describeSnapshotCopyGrants",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSnapshotCopyGrants?Marker=Marker&MaxRecords=MaxRecords&SnapshotCopyGrantName=SnapshotCopyGrantName&TagKeys.TagKey.N=TagKeys.TagKey.N&TagValues.TagValue.N=TagValues.TagValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of snapshot copy grants owned by the AWS account in the destination\n            region."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34a0e954-9cf4-4b5e-972a-03ac862d5431"
            }
          ]
        },
        {
          "id": "55a4382e-63bf-4a2f-8c11-e7d0ce1afbb6",
          "name": "disableSnapshotCopy",
          "request": {
            "url": "http://example.com/api/?Action=DisableSnapshotCopy?ClusterIdentifier=ClusterIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables the automatic copying of snapshots from one region to another region for a\n            specified cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c436d325-ce23-430a-8e1c-57a41175bd03"
            }
          ]
        },
        {
          "id": "0a16d246-f2cb-4ce1-8a67-3b9e0e8baf2a",
          "name": "enableSnapshotCopy",
          "request": {
            "url": "http://example.com/api/?Action=EnableSnapshotCopy?ClusterIdentifier=ClusterIdentifier&DestinationRegion=DestinationRegion&RetentionPeriod=RetentionPeriod&SnapshotCopyGrantName=SnapshotCopyGrantName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables the automatic copy of snapshots from one region to another region for a\n            specified cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3bdd4e8b-3526-49d3-a1af-6ce8a4a19781"
            }
          ]
        }
      ]
    },
    {
      "name": "Clusters",
      "item": [
        {
          "id": "fbae386a-f226-40af-a8fe-be76607f536d",
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
              "id": "9635704b-22cc-41e6-a491-ab23efcf46ac"
            }
          ]
        },
        {
          "id": "d6ab461e-3336-4f92-bdef-6264f26a0577",
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
              "id": "fa473b28-f19f-4c97-b53d-38eab56f5862"
            }
          ]
        },
        {
          "id": "06eed1a9-0bf1-4deb-9a64-0d8e18dae875",
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
              "id": "fe23faa3-07c6-4f00-8eca-5ef44ffcce68"
            }
          ]
        },
        {
          "id": "26d180f6-51b9-4bdb-8a89-423001c887cc",
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
              "id": "ed269b57-c398-4529-aed3-fb07b97044f6"
            }
          ]
        },
        {
          "id": "d30d298c-b527-408f-a6fa-452e868810c1",
          "name": "modifyCluster",
          "request": {
            "url": "http://example.com/api/?Action=ModifyCluster?AllowVersionUpgrade=AllowVersionUpgrade&AutomatedSnapshotRetentionPeriod=AutomatedSnapshotRetentionPeriod&ClusterIdentifier=ClusterIdentifier&ClusterParameterGroupName=ClusterParameterGroupName&ClusterSecurityGroups.ClusterSecurityGroupName.N=ClusterSecurityGroups.ClusterSecurityGroupName.N&ClusterType=ClusterType&ClusterVersion=ClusterVersion&ElasticIp=ElasticIp&EnhancedVpcRouting=EnhancedVpcRouting&HsmClientCertificateIdentifier=HsmClientCertificateIdentifier&HsmConfigurationIdentifier=HsmConfigurationIdentifier&MasterUserPassword=MasterUserPassword&NewClusterIdentifier=NewClusterIdentifier&NodeType=NodeType&NumberOfNodes=NumberOfNodes&PreferredMaintenanceWindow=PreferredMaintenanceWindow&PubliclyAccessible=PubliclyAccessible&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the settings for a cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52518bf3-c619-46a2-afbe-2f0cb0ff8de5"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameter Groups",
      "item": [
        {
          "id": "39ead6e7-a02d-4cfe-b17b-43bac0df5afa",
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
              "id": "6c9a618c-fc1b-4789-b0ec-8be69c6e1699"
            }
          ]
        },
        {
          "id": "c4248b75-3773-4f46-aba9-25428ac59949",
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
              "id": "732c9c2c-82d1-4273-8611-de4665f0381d"
            }
          ]
        },
        {
          "id": "22a7b180-0105-4039-a2ed-b63be3ed8ab0",
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
              "id": "7900a004-7c84-4611-80d2-7f8beb91ad73"
            }
          ]
        },
        {
          "id": "a6530d0c-bfc3-49f4-9276-fc5c1ee3f8f8",
          "name": "modifyClusterParameterGroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyClusterParameterGroup?ParameterGroupName=ParameterGroupName&Parameters.Parameter.N=Parameters.Parameter.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the parameters of a parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36f4b108-158f-4a0c-998c-c73c92ba3b82"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Subnet Groups",
      "item": [
        {
          "id": "a4871add-43ff-4e2d-815e-f8a4f22ac363",
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
              "id": "85e35704-956c-4a22-9b3c-202dcb1a57ab"
            }
          ]
        },
        {
          "id": "eb59e883-5d55-4ab4-b475-1340e0a5d199",
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
              "id": "f2e0dc56-f9e8-42a2-af95-2906db67611c"
            }
          ]
        },
        {
          "id": "d2f04d9e-99bd-4110-a06e-267ee109098d",
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
              "id": "9d752d69-4986-48ef-9657-5e9fb0ee6644"
            }
          ]
        },
        {
          "id": "ccd50315-8756-4981-809c-9c1e9fe3aa07",
          "name": "modifyClusterSubnetGroup",
          "request": {
            "url": "http://example.com/api/?Action=ModifyClusterSubnetGroup?ClusterSubnetGroupName=ClusterSubnetGroupName&Description=Description&SubnetIds.SubnetIdentifier.N=SubnetIds.SubnetIdentifier.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies a cluster subnet group to include the specified list of VPC subnets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b91f6701-bb4b-4dc0-ac73-6bca359b333d"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "8137b02e-01ae-4b8c-80cd-5c94b035e2be",
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
              "id": "83b45d2f-7edd-480e-922e-38918b8a268b"
            }
          ]
        },
        {
          "id": "6e28090d-37c1-487c-80d0-ee3f28be228c",
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
              "id": "cdb07cb9-0209-4f46-b831-b56815c4ea39"
            }
          ]
        },
        {
          "id": "c147f80d-12b7-40bc-8014-e9a128df3bc6",
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
              "id": "b84b4737-8cbc-4a41-9f9e-7236ac679ce1"
            }
          ]
        },
        {
          "id": "114a7aad-b4d3-4d82-9001-3063edd5921e",
          "name": "modifyEventSubscription",
          "request": {
            "url": "http://example.com/api/?Action=ModifyEventSubscription?Enabled=Enabled&EventCategories.EventCategory.N=EventCategories.EventCategory.N&Severity=Severity&SnsTopicArn=SnsTopicArn&SourceIds.SourceId.N=SourceIds.SourceId.N&SourceType=SourceType&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies an existing Amazon Redshift event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3887abf0-68e0-49ba-a689-eb056a2cb3db"
            }
          ]
        }
      ]
    },
    {
      "name": "HSM Client Certificates",
      "item": [
        {
          "id": "d4c65500-45a0-44e2-b6b2-5f9ab27aee46",
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
              "id": "63b9e58b-7a3e-4f7e-b6f4-133bae7827ee"
            }
          ]
        },
        {
          "id": "67f0f27f-a016-4bfd-9402-6b1ab8bd4e47",
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
              "id": "3aa4f877-1543-4391-bb9b-2dbb21fcc572"
            }
          ]
        },
        {
          "id": "ae5493a6-a669-464f-aefb-2cbd53a30ffa",
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
              "id": "ca77af22-45b3-425d-8391-add05f7be49e"
            }
          ]
        }
      ]
    },
    {
      "name": "HSM Configurations",
      "item": [
        {
          "id": "39354781-e7fb-404a-806c-ac8363c1b4a2",
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
              "id": "97539c34-840e-448d-aeb9-6a27cdb0cfa9"
            }
          ]
        },
        {
          "id": "3b61b2e8-e267-4369-87cb-a5cb8949c4af",
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
              "id": "35b6b7f9-12c4-42b6-b083-0b70349af1a1"
            }
          ]
        },
        {
          "id": "7654c9a7-2583-4431-a5d2-eb8cef69edb7",
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
              "id": "034b9114-2941-4a8d-b265-bf72f760a4e2"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "71b2790a-4cf7-463b-84bc-df351a4cbfe8",
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
              "id": "eb6a2a8b-3332-401f-96ba-f7cd711954ed"
            }
          ]
        },
        {
          "id": "20a46d5e-ac18-4807-9bec-7cdbc8c1dc56",
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
              "id": "f47e2d41-369d-4337-886e-ff4d2b6a3c1b"
            }
          ]
        },
        {
          "id": "cda463b1-9bd6-4a39-bdba-936d2643344d",
          "name": "describeTags",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTags?Marker=Marker&MaxRecords=MaxRecords&ResourceName=ResourceName&ResourceType=ResourceType&TagKeys.TagKey.N=TagKeys.TagKey.N&TagValues.TagValue.N=TagValues.TagValue.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08e0d0c2-a120-43a0-a313-9b846e5886a0"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameters",
      "item": [
        {
          "id": "31cd9a1e-b5cf-4fd4-a3df-4709a0f94635",
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
              "id": "b356952a-9595-47e1-9d37-c4fcb43e0579"
            }
          ]
        },
        {
          "id": "0823e50c-3571-42e7-91e6-2597a96e12bb",
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
              "id": "9c28ba1f-aef2-411f-a0d6-a47739f4a05a"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Categories",
      "item": [
        {
          "id": "e5cf3647-63a1-49c3-8d5f-a28e8b66f732",
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
              "id": "187002d6-4aae-4d53-ae99-ce9a904eea5d"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "a2846f87-9f6b-4fa1-a101-f4dbe2a1e010",
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
              "id": "8b2adaed-843e-4113-99de-02412f0fa809"
            }
          ]
        }
      ]
    },
    {
      "name": "Logging",
      "item": [
        {
          "id": "cf41951b-2d01-451e-a09f-f6aec2d358c3",
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
              "id": "c07da8f9-eff9-4b6a-93d2-304fdc18b403"
            }
          ]
        },
        {
          "id": "532e8edf-205a-4fc6-a63f-d705e90a9251",
          "name": "disableLogging",
          "request": {
            "url": "http://example.com/api/?Action=DisableLogging?ClusterIdentifier=ClusterIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Stops logging information, such as queries and connection attempts, for the\n            specified Amazon Redshift cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b14f9398-39f4-4d21-9af6-526d580d8ee6"
            }
          ]
        },
        {
          "id": "9e6980e4-04a6-42b0-8902-c1adb286ae98",
          "name": "enableLogging",
          "request": {
            "url": "http://example.com/api/?Action=EnableLogging?BucketName=BucketName&ClusterIdentifier=ClusterIdentifier&S3KeyPrefix=S3KeyPrefix",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts logging information, such as queries and connection attempts, for the\n            specified Amazon Redshift cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44723a8d-3f20-45c7-ba20-bd884d283933"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Options",
      "item": [
        {
          "id": "82bbfd74-f4ce-47d2-9e46-deaf749a0266",
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
              "id": "435936f4-aaa2-48a4-99d6-78dc6123bc6e"
            }
          ]
        }
      ]
    },
    {
      "name": "Reserved Nodes",
      "item": [
        {
          "id": "e352ad1b-ed38-4df2-83c0-a289d362beff",
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
              "id": "a90a9d16-d081-4fff-9fd0-614cde951ca4"
            }
          ]
        },
        {
          "id": "3fdf2a91-71c3-4e43-bb33-23762a14eba3",
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
              "id": "0264133d-e488-4120-844a-b11b20869969"
            }
          ]
        }
      ]
    },
    {
      "name": "Resize",
      "item": [
        {
          "id": "c9bcb329-b4b6-499b-bff1-7f5fa8304353",
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
              "id": "ab825bbe-c4eb-4383-80fb-6485120892e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Tables",
      "item": [
        {
          "id": "96bcd7d0-66aa-4780-88ed-782d2f27f1dc",
          "name": "describeTableRestoreStatus",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTableRestoreStatus?ClusterIdentifier=ClusterIdentifier&Marker=Marker&MaxRecords=MaxRecords&TableRestoreRequestId=TableRestoreRequestId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the status of one or more table restore requests made using the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b951f003-2983-490f-a479-967f027f2b6c"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster IAM Roles",
      "item": [
        {
          "id": "fcda3614-ce59-42e6-83aa-5ab7e60dba19",
          "name": "modifyClusterIamRoles",
          "request": {
            "url": "http://example.com/api/?Action=ModifyClusterIamRoles?AddIamRoles.IamRoleArn.N=AddIamRoles.IamRoleArn.N&ClusterIdentifier=ClusterIdentifier&RemoveIamRoles.IamRoleArn.N=RemoveIamRoles.IamRoleArn.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Modifies the list of AWS Identity and Access Management (IAM) roles that can be\n            used by the cluster to access other AWS services."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc9c2ab6-665c-49eb-a047-740d15d7b30e"
            }
          ]
        }
      ]
    }
  ]
}