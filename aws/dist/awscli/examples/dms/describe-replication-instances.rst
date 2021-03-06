**To describe replication instances**

The following ``describe-replication-instances`` example lists the replication instances in your AWS account. ::

    aws dms describe-replication-instances

Output::

    {
        "ReplicationInstances": [
            {
                "ReplicationInstanceIdentifier": "my-repl-instance",
                "ReplicationInstanceClass": "dms.t2.micro",
                "ReplicationInstanceStatus": "available",
                "AllocatedStorage": 5,
                "InstanceCreateTime": 1590011235.952,
                "VpcSecurityGroups": [
                    {
                        "VpcSecurityGroupId": "sg-f839b688",
                        "Status": "active"
                    }
                ],
                "AvailabilityZone": "us-east-1e",
                "ReplicationSubnetGroup": {
                    "ReplicationSubnetGroupIdentifier": "default",
                    "ReplicationSubnetGroupDescription": "default",
                    "VpcId": "vpc-136a4c6a",
                    "SubnetGroupStatus": "Complete",
                    "Subnets": [
                        {
                            "SubnetIdentifier": "subnet-da327bf6",
                            "SubnetAvailabilityZone": {
                                "Name": "us-east-1a"
                            },
                            "SubnetStatus": "Active"
                        },
                        {
                            "SubnetIdentifier": "subnet-42599426",
                            "SubnetAvailabilityZone": {
                                "Name": "us-east-1d"
                            },
                            "SubnetStatus": "Active"
                        },
                        {
                            "SubnetIdentifier": "subnet-bac383e0",
                            "SubnetAvailabilityZone": {
                                "Name": "us-east-1c"
                            },
                            "SubnetStatus": "Active"
                        },
                        {
                            "SubnetIdentifier": "subnet-6746046b",
                            "SubnetAvailabilityZone": {
                                "Name": "us-east-1f"
                            },
                            "SubnetStatus": "Active"
                        },
                        {
                            "SubnetIdentifier": "subnet-d7c825e8",
                            "SubnetAvailabilityZone": {
                                "Name": "us-east-1e"
                            },
                            "SubnetStatus": "Active"
                        },
                        {
                            "SubnetIdentifier": "subnet-cbfff283",
                            "SubnetAvailabilityZone": {
                                "Name": "us-east-1b"
                            },
                            "SubnetStatus": "Active"
                        }
                    ]
                },
                "PreferredMaintenanceWindow": "wed:11:42-wed:12:12",
                "PendingModifiedValues": {
                    "MultiAZ": true
                },
                "MultiAZ": false,
                "EngineVersion": "3.3.2",
                "AutoMinorVersionUpgrade": true,
                "KmsKeyId": "arn:aws:kms:us-east-1:123456789012:key/f7bc0f8e-1a3a-4ace-9faa-e8494fa3921a",
                "ReplicationInstanceArn": "arn:aws:dms:us-east-1:123456789012:rep:T3OM7OUB5NM2LCVZF7JPGJRNUE",
                "ReplicationInstancePublicIpAddress": "3.230.18.248",
                "ReplicationInstancePrivateIpAddress": "172.31.75.90",
                "ReplicationInstancePublicIpAddresses": [
                    "3.230.18.248"
                ],
                "ReplicationInstancePrivateIpAddresses": [
                    "172.31.75.90"
                ],
                "PubliclyAccessible": true,
                "FreeUntil": 1590194829.267
            }
        ]
    }

For more information, see `Working with an AWS DMS Replication Instance <https://docs.aws.amazon.com/dms/latest/userguide/CHAP_ReplicationInstance.html>`__ in the *AWS Database Migration Service User Guide*.
