{
  "info": {
    "name": "Amazon Redshift API Create Event Subscription",
    "_postman_id": "62c5624b-ee2e-4682-ab82-4e965f6b8c18",
    "description": "Creates an Amazon Redshift event notification subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Cluster Security Group",
      "item": [
        {
          "id": "63290968-bae2-4e73-9ea6-2f95698b9797",
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
              "id": "909fd017-071e-4ece-b040-b446870811ab"
            }
          ]
        },
        {
          "id": "30b9230d-45f0-4580-b26c-b9c888d18c14",
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
              "id": "54c8ae69-d273-431e-bcbc-7b8c5d65e945"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "f2feb2b9-c009-43f0-9218-2c698744caa2",
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
              "id": "d7ade8ec-c75f-42b2-96c0-303e80ebeb61"
            }
          ]
        },
        {
          "id": "a2ef3ae7-71e4-491d-9e16-8b107d32473f",
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
              "id": "c7c543d4-5c7c-4b7e-ac90-596ecde0760a"
            }
          ]
        },
        {
          "id": "26218990-4ba3-4f25-8a04-3b5df66f63d1",
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
              "id": "9cbd7eab-ae1a-4254-8ce5-05f2b8a1c593"
            }
          ]
        }
      ]
    },
    {
      "name": "Clusters",
      "item": [
        {
          "id": "db9dd055-5f28-40c3-974b-b33a3c073921",
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
              "id": "013866dd-f6c1-4d06-86be-41d0df02b40f"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameter Groups",
      "item": [
        {
          "id": "6218d2b4-ca1e-4c1d-9e77-48205582823f",
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
              "id": "4ffe0841-9030-4a69-ab43-ee72ca3c487e"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Subnet Groups",
      "item": [
        {
          "id": "8937cf41-9b56-4d95-b40a-41337c63cddd",
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
              "id": "02f55813-a663-43be-92f7-943fa69ada27"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "57987e9b-b894-49c3-a959-8cfc8b47cf9c",
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
              "id": "f28052c9-2ce1-4a4d-b807-96cd59987680"
            }
          ]
        }
      ]
    }
  ]
}