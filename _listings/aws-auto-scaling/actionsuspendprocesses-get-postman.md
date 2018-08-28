{
  "info": {
    "name": "AWS Auto Scaling API Suspend Processes",
    "_postman_id": "7779b3cf-1137-48fc-bbf9-724d4df7190a",
    "description": "Suspends the specified Auto Scaling processes, or all processes, for the specified Auto Scaling group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Server Instance",
      "item": [
        {
          "id": "e7c7fa98-9429-40e0-8885-cc4de377f233",
          "name": "attachInstances",
          "request": {
            "url": "http://example.com/api/?Action=AttachInstances?AutoScalingGroupName=AutoScalingGroupName&InstanceIds.member.N=InstanceIds.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches one or more EC2 instances to the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c05c394-d9fc-46b1-9a23-fa6378da8002"
            }
          ]
        }
      ]
    },
    {
      "name": "Load Balancers",
      "item": [
        {
          "id": "0a52caac-510b-477b-9b16-f5d10f662f06",
          "name": "attachLoadBalancers",
          "request": {
            "url": "http://example.com/api/?Action=AttachLoadBalancers?AutoScalingGroupName=AutoScalingGroupName&LoadBalancerNames.member.N=LoadBalancerNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches one or more Classic load balancers to the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d239fcd9-d9ab-4288-a4eb-7ff57f56751b"
            }
          ]
        },
        {
          "id": "0e021b96-7ae8-49ed-b5d6-c084fa2b2b1d",
          "name": "attachLoadBalancerTargetGroups",
          "request": {
            "url": "http://example.com/api/?Action=AttachLoadBalancerTargetGroups?AutoScalingGroupName=AutoScalingGroupName&TargetGroupARNs.member.N=TargetGroupARNs.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches one or more target groups to the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8985b95f-d812-47e9-a418-e174a47ed75b"
            }
          ]
        },
        {
          "id": "74babecd-ac33-4ed4-baeb-1ef3df91669a",
          "name": "describeLoadBalancers",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLoadBalancers?AutoScalingGroupName=AutoScalingGroupName&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the load balancers for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ae0d748-e110-45dd-9219-11ba569125d8"
            }
          ]
        },
        {
          "id": "8d48a7df-40e7-4c0e-bde6-65c629a7a90a",
          "name": "describeLoadBalancerTargetGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLoadBalancerTargetGroups?AutoScalingGroupName=AutoScalingGroupName&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the target groups for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09754a2b-b4f5-43b6-a168-b19a98c91b98"
            }
          ]
        },
        {
          "id": "f763dd13-1a81-42de-a93a-ffea7dba70de",
          "name": "detachLoadBalancers",
          "request": {
            "url": "http://example.com/api/?Action=DetachLoadBalancers?AutoScalingGroupName=AutoScalingGroupName&LoadBalancerNames.member.N=LoadBalancerNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Detaches one or more Classic load balancers from the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5a117f2-781a-4de6-90c8-00ab28cd8efb"
            }
          ]
        },
        {
          "id": "34233e58-1735-4ee2-81b4-2158f4b00443",
          "name": "detachLoadBalancerTargetGroups",
          "request": {
            "url": "http://example.com/api/?Action=DetachLoadBalancerTargetGroups?AutoScalingGroupName=AutoScalingGroupName&TargetGroupARNs.member.N=TargetGroupARNs.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Detaches one or more target groups from the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "435e39d1-a430-410f-809f-e7e97ba86406"
            }
          ]
        }
      ]
    },
    {
      "name": "Life Cycle",
      "item": [
        {
          "id": "7ba2d08b-8094-4e2f-9e39-c29354d65d41",
          "name": "completeLifecycleAction",
          "request": {
            "url": "http://example.com/api/?Action=CompleteLifecycleAction?AutoScalingGroupName=AutoScalingGroupName&InstanceId=InstanceId&LifecycleActionResult=LifecycleActionResult&LifecycleActionToken=LifecycleActionToken&LifecycleHookName=LifecycleHookName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Completes the lifecycle action for the specified token or instance with the specified result."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8cec7c9c-8d88-46ae-abd3-857713b63764"
            }
          ]
        },
        {
          "id": "11ec5342-059b-4e26-a71b-bf5741c80e23",
          "name": "deleteLifecycleHook",
          "request": {
            "url": "http://example.com/api/?Action=DeleteLifecycleHook?AutoScalingGroupName=AutoScalingGroupName&LifecycleHookName=LifecycleHookName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified lifecycle hook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7268f2c9-302c-4380-bb3d-071a6f63c821"
            }
          ]
        },
        {
          "id": "afd82a8a-19de-487e-bc73-e2142379242f",
          "name": "describeLifecycleHooks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLifecycleHooks?AutoScalingGroupName=AutoScalingGroupName&LifecycleHookNames.member.N=LifecycleHookNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the lifecycle hooks for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f3ca754-7eaa-4f6f-b54f-44fbfab073d8"
            }
          ]
        },
        {
          "id": "d64b3278-03f1-44b6-99aa-eb4eba6506e2",
          "name": "describeLifecycleHookTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLifecycleHookTypes?LifecycleHookTypes.member.N=LifecycleHookTypes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the available types of lifecycle hooks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2c5b286-0fe6-464d-a20b-a28ef565a306"
            }
          ]
        },
        {
          "id": "952a688c-c72e-40ad-aba5-e97ae93eb3f2",
          "name": "putLifecycleHook",
          "request": {
            "url": "http://example.com/api/?Action=PutLifecycleHook?AutoScalingGroupName=AutoScalingGroupName&DefaultResult=DefaultResult&HeartbeatTimeout=HeartbeatTimeout&LifecycleHookName=LifecycleHookName&LifecycleTransition=LifecycleTransition&NotificationMetadata=NotificationMetadata&NotificationTargetARN=NotificationTargetARN&RoleARN=RoleARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates or updates a lifecycle hook for the specified Auto Scaling Group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d21e33d1-00bf-4034-a4d2-c52ab84ca279"
            }
          ]
        },
        {
          "id": "72455209-0283-436d-bf79-42b92da2fc86",
          "name": "recordLifecycleActionHeartbeat",
          "request": {
            "url": "http://example.com/api/?Action=RecordLifecycleActionHeartbeat?AutoScalingGroupName=AutoScalingGroupName&InstanceId=InstanceId&LifecycleActionToken=LifecycleActionToken&LifecycleHookName=LifecycleHookName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Records a heartbeat for the lifecycle action associated with the specified token or instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34722ca2-1707-47ad-8289-2378cfbe8ba9"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto Scaling Groups",
      "item": [
        {
          "id": "fb88c202-d31c-4952-bccd-fc4a24f8cea1",
          "name": "createAutoScalingGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateAutoScalingGroup?AutoScalingGroupName=AutoScalingGroupName&AvailabilityZones.member.N=AvailabilityZones.member.N&DefaultCooldown=DefaultCooldown&DesiredCapacity=DesiredCapacity&HealthCheckGracePeriod=HealthCheckGracePeriod&HealthCheckType=HealthCheckType&InstanceId=InstanceId&LaunchConfigurationName=LaunchConfigurationName&LoadBalancerNames.member.N=LoadBalancerNames.member.N&MaxSize=MaxSize&MinSize=MinSize&NewInstancesProtectedFromScaleIn=NewInstancesProtectedFromScaleIn&PlacementGroup=PlacementGroup&Tags.member.N=Tags.member.N&TargetGroupARNs.member.N=TargetGroupARNs.member.N&TerminationPolicies.member.N=TerminationPolicies.member.N&VPCZoneIdentifier=VPCZoneIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an Auto Scaling group with the specified name and attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a0b3e77-a6d7-4758-8b05-95d9b62ce232"
            }
          ]
        },
        {
          "id": "d6dd23f6-edad-4a80-a23d-c45948182482",
          "name": "deleteAutoScalingGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAutoScalingGroup?AutoScalingGroupName=AutoScalingGroupName&ForceDelete=ForceDelete",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9fb91fca-4bb9-4dc3-bf50-f38d3887ca6a"
            }
          ]
        },
        {
          "id": "47a36b4c-8170-4c72-bc59-31134f1441f7",
          "name": "describeAutoScalingGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutoScalingGroups?AutoScalingGroupNames.member.N=AutoScalingGroupNames.member.N&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more Auto Scaling groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "397b32bf-45ff-4c52-855f-63d65c23cf21"
            }
          ]
        }
      ]
    },
    {
      "name": "Launch",
      "item": [
        {
          "id": "ccce1a3c-4664-4610-b328-e7bd152039e9",
          "name": "createLaunchConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=CreateLaunchConfiguration?AssociatePublicIpAddress=AssociatePublicIpAddress&BlockDeviceMappings.member.N=BlockDeviceMappings.member.N&ClassicLinkVPCId=ClassicLinkVPCId&ClassicLinkVPCSecurityGroups.member.N=ClassicLinkVPCSecurityGroups.member.N&EbsOptimized=EbsOptimized&IamInstanceProfile=IamInstanceProfile&ImageId=ImageId&InstanceId=InstanceId&InstanceMonitoring=InstanceMonitoring&InstanceType=InstanceType&KernelId=KernelId&KeyName=KeyName&LaunchConfigurationName=LaunchConfigurationName&PlacementTenancy=PlacementTenancy&RamdiskId=RamdiskId&SecurityGroups.member.N=SecurityGroups.member.N&SpotPrice=SpotPrice&UserData=UserData",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a launch configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b933d19-fb15-475c-8f79-14928036c09e"
            }
          ]
        },
        {
          "id": "db2fffe7-1a54-4a2e-aa6a-8dd1e3b007b2",
          "name": "deleteLaunchConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=DeleteLaunchConfiguration?LaunchConfigurationName=LaunchConfigurationName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified launch configuration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d68ad36f-80cf-4c5e-ac8b-ef999d1f3d22"
            }
          ]
        },
        {
          "id": "3bcd16bf-7007-4e67-92e2-bd36f8394458",
          "name": "describeLaunchConfigurations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeLaunchConfigurations?LaunchConfigurationNames.member.N=LaunchConfigurationNames.member.N&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more launch configurations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "329332ea-fccb-48b6-b5b6-9d50b958b558"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "c65d594e-724a-4e9c-8b5b-95a6b3409a43",
          "name": "createOrUpdateTags",
          "request": {
            "url": "http://example.com/api/?Action=CreateOrUpdateTags?Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates or updates tags for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "159c10f1-de58-4800-9a52-894871d68947"
            }
          ]
        },
        {
          "id": "c02fe465-d005-4ed4-9b21-2d74428e6628",
          "name": "deleteTags",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTags?Tags.member.N=Tags.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ab2b7eb-ec23-42c8-bac5-928ef373bdad"
            }
          ]
        },
        {
          "id": "7f71cc5f-1e01-4449-9cbf-41127a7d80c2",
          "name": "describeTags",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTags?Filters.member.N=Filters.member.N&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified tags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f0b33d8-afc3-4827-9319-f16971a08489"
            }
          ]
        }
      ]
    },
    {
      "name": "Notifications",
      "item": [
        {
          "id": "ba8c1fda-383f-4985-b9db-f18f9553898d",
          "name": "deleteNotificationConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=DeleteNotificationConfiguration?AutoScalingGroupName=AutoScalingGroupName&TopicARN=TopicARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified notification."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df3eca63-c146-40b2-8ca2-f78b2fd3368c"
            }
          ]
        },
        {
          "id": "266a3540-d88a-4547-861e-bf3de1c2e3f7",
          "name": "describeNotificationConfigurations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeNotificationConfigurations?AutoScalingGroupNames.member.N=AutoScalingGroupNames.member.N&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the notification actions associated with the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c34a3d6-400e-4664-bd35-8c7cca2ac525"
            }
          ]
        },
        {
          "id": "f8b691f0-ebe8-42a7-b107-d6026b9fc2db",
          "name": "putNotificationConfiguration",
          "request": {
            "url": "http://example.com/api/?Action=PutNotificationConfiguration?AutoScalingGroupName=AutoScalingGroupName&NotificationTypes.member.N=NotificationTypes.member.N&TopicARN=TopicARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures an Auto Scaling group to send notifications when specified events take place."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de71d598-448a-4cac-9ab6-8b743cd32f90"
            }
          ]
        }
      ]
    },
    {
      "name": "Policies",
      "item": [
        {
          "id": "299d348b-b274-404b-99dd-0a8d87aecbbd",
          "name": "deletePolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeletePolicy?AutoScalingGroupName=AutoScalingGroupName&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Auto Scaling policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a360371-d782-486d-922e-1623f59da4b4"
            }
          ]
        },
        {
          "id": "daa7cd36-b65e-4d88-b20b-eb37b5de0fcd",
          "name": "describePolicies",
          "request": {
            "url": "http://example.com/api/?Action=DescribePolicies?AutoScalingGroupName=AutoScalingGroupName&MaxRecords=MaxRecords&NextToken=NextToken&PolicyNames.member.N=PolicyNames.member.N&PolicyTypes.member.N=PolicyTypes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the policies for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "306d63bb-8329-498e-857c-2d6a270475e5"
            }
          ]
        },
        {
          "id": "a1d0122b-e819-444b-b72d-532fc3507714",
          "name": "executePolicy",
          "request": {
            "url": "http://example.com/api/?Action=ExecutePolicy?AutoScalingGroupName=AutoScalingGroupName&BreachThreshold=BreachThreshold&HonorCooldown=HonorCooldown&MetricValue=MetricValue&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Executes the specified policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0efa895-3c2a-4321-88cd-cd6ec93367c3"
            }
          ]
        }
      ]
    },
    {
      "name": "Scheduled Action",
      "item": [
        {
          "id": "687bde69-19ce-499b-a7bf-6ec3251180ed",
          "name": "deleteScheduledAction",
          "request": {
            "url": "http://example.com/api/?Action=DeleteScheduledAction?AutoScalingGroupName=AutoScalingGroupName&ScheduledActionName=ScheduledActionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified scheduled action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b759502b-8ce0-4f43-a211-c5f56bd8d923"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Limits",
      "item": [
        {
          "id": "8e056cbd-74ba-4d25-a64b-2f84ab49baff",
          "name": "describeAccountLimits",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAccountLimits?MaxNumberOfAutoScalingGroups=MaxNumberOfAutoScalingGroups&MaxNumberOfLaunchConfigurations=MaxNumberOfLaunchConfigurations&NumberOfAutoScalingGroups=NumberOfAutoScalingGroups&NumberOfLaunchConfigurations=NumberOfLaunchConfigurations",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the current Auto Scaling resource limits for your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef7f4a1b-0c6a-4f5c-847e-ae8ab2f2d9b5"
            }
          ]
        }
      ]
    },
    {
      "name": "Adjustment Types",
      "item": [
        {
          "id": "955abc7d-67ff-4a4b-ac0f-c68e446501d8",
          "name": "describeAdjustmentTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAdjustmentTypes?AdjustmentTypes.member.N=AdjustmentTypes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the policy adjustment types for use with."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3464ee13-292a-415d-8a85-3ae5ca3bb9ae"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto Scaling Instances",
      "item": [
        {
          "id": "4967fcbf-e141-4922-a163-577d52a5aecd",
          "name": "describeAutoScalingInstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutoScalingInstances?InstanceIds.member.N=InstanceIds.member.N&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more Auto Scaling instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02c6c433-b28a-4ce2-8b08-0690e59858a6"
            }
          ]
        }
      ]
    },
    {
      "name": "Auto Scaling Notifications",
      "item": [
        {
          "id": "4f0b5852-31f7-4dd5-85fb-89dafa96411c",
          "name": "describeAutoScalingNotificationTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutoScalingNotificationTypes?AutoScalingNotificationTypes.member.N=AutoScalingNotificationTypes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the notification types that are supported by Auto Scaling."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6688697-e8e4-4785-be38-339e0a009a4b"
            }
          ]
        }
      ]
    },
    {
      "name": "Metric Collection",
      "item": [
        {
          "id": "52ec8ab6-99fe-477a-aa5f-12389f73e6a7",
          "name": "describeMetricCollectionTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMetricCollectionTypes?Granularities.member.N=Granularities.member.N&Metrics.member.N=Metrics.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the available CloudWatch metrics for Auto Scaling."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d7bd98e-d714-4ca8-ac2f-a699412226f7"
            }
          ]
        }
      ]
    },
    {
      "name": "Scaling Activities",
      "item": [
        {
          "id": "25afc0e8-0d88-484d-921d-e4dc063443ba",
          "name": "describeScalingActivities",
          "request": {
            "url": "http://example.com/api/?Action=DescribeScalingActivities?ActivityIds.member.N=ActivityIds.member.N&AutoScalingGroupName=AutoScalingGroupName&MaxRecords=MaxRecords&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more scaling activities for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4483ee4-0d5e-4695-af26-2cc4a5bc2101"
            }
          ]
        }
      ]
    },
    {
      "name": "Scaling Process",
      "item": [
        {
          "id": "8020e47e-7338-46de-8b4d-5356b5fd1353",
          "name": "describeScalingProcessTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeScalingProcessTypes?Processes.member.N=Processes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the scaling process types for use with."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d9fd5bd-3b6c-4817-a154-a6c916fbb57d"
            }
          ]
        }
      ]
    },
    {
      "name": "Scheduled Actions",
      "item": [
        {
          "id": "df3eb168-0c5c-48f9-af2d-59858ce79db5",
          "name": "describeScheduledActions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeScheduledActions?AutoScalingGroupName=AutoScalingGroupName&EndTime=EndTime&MaxRecords=MaxRecords&NextToken=NextToken&ScheduledActionNames.member.N=ScheduledActionNames.member.N&StartTime=StartTime",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the actions scheduled for your Auto Scaling group that haven't run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42910d69-b568-4b59-958f-0de0ee8fd606"
            }
          ]
        }
      ]
    },
    {
      "name": "Termination Policies",
      "item": [
        {
          "id": "6aed0935-015e-4d3c-9901-f7d3a49afda9",
          "name": "describeTerminationPolicyTypes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTerminationPolicyTypes?TerminationPolicyTypes.member.N=TerminationPolicyTypes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the termination policies supported by Auto Scaling."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f55c5a2-c22b-4970-9701-ba38463cb215"
            }
          ]
        }
      ]
    },
    {
      "name": "Server Instances",
      "item": [
        {
          "id": "12536aa7-c225-4719-af58-03c4666ac821",
          "name": "detachInstances",
          "request": {
            "url": "http://example.com/api/?Action=DetachInstances?AutoScalingGroupName=AutoScalingGroupName&InstanceIds.member.N=InstanceIds.member.N&ShouldDecrementDesiredCapacity=ShouldDecrementDesiredCapacity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes one or more instances from the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88f7534e-2984-422a-9ddb-f0b25d2f497b"
            }
          ]
        }
      ]
    },
    {
      "name": "Metrics Collection",
      "item": [
        {
          "id": "5f19067a-3c2b-487e-9922-a7d2a957d8a6",
          "name": "disableMetricsCollection",
          "request": {
            "url": "http://example.com/api/?Action=DisableMetricsCollection?AutoScalingGroupName=AutoScalingGroupName&Metrics.member.N=Metrics.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables group metrics for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed5ba997-0a09-4ff5-a23f-0d40ffeea607"
            }
          ]
        },
        {
          "id": "0ffa349a-6608-476e-8e9c-2c300b005a1d",
          "name": "enableMetricsCollection",
          "request": {
            "url": "http://example.com/api/?Action=EnableMetricsCollection?AutoScalingGroupName=AutoScalingGroupName&Granularity=Granularity&Metrics.member.N=Metrics.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables group metrics for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8231d57-3ec8-4467-abbe-5ccf09f23410"
            }
          ]
        }
      ]
    },
    {
      "name": "Stand By",
      "item": [
        {
          "id": "1e88410d-beb5-468c-a757-4831a27ee9e2",
          "name": "enterStandby",
          "request": {
            "url": "http://example.com/api/?Action=EnterStandby?AutoScalingGroupName=AutoScalingGroupName&InstanceIds.member.N=InstanceIds.member.N&ShouldDecrementDesiredCapacity=ShouldDecrementDesiredCapacity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Moves the specified instances into Standby mode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ccbf48e-bb7a-454a-b042-fd08c6ded352"
            }
          ]
        },
        {
          "id": "6a67af00-c903-438e-8a69-37bb01e23ec5",
          "name": "exitStandby",
          "request": {
            "url": "http://example.com/api/?Action=ExitStandby?AutoScalingGroupName=AutoScalingGroupName&InstanceIds.member.N=InstanceIds.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Moves the specified instances out of Standby mode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b553bdd0-9ae0-4707-be68-c3ba9568b1a4"
            }
          ]
        }
      ]
    },
    {
      "name": "Scaling Policy",
      "item": [
        {
          "id": "3c3d3b9c-6c6a-4855-ba5e-8e7824ac304b",
          "name": "putScalingPolicy",
          "request": {
            "url": "http://example.com/api/?Action=PutScalingPolicy?AdjustmentType=AdjustmentType&AutoScalingGroupName=AutoScalingGroupName&Cooldown=Cooldown&EstimatedInstanceWarmup=EstimatedInstanceWarmup&MetricAggregationType=MetricAggregationType&MinAdjustmentMagnitude=MinAdjustmentMagnitude&MinAdjustmentStep=MinAdjustmentStep&PolicyName=PolicyName&PolicyType=PolicyType&ScalingAdjustment=ScalingAdjustment&StepAdjustments.member.N=StepAdjustments.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates or updates a policy for an Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5ea82b6-aedf-4158-a0e1-1114cf032713"
            }
          ]
        }
      ]
    },
    {
      "name": "Scheduled Update",
      "item": [
        {
          "id": "5beeb0b9-7dae-406b-a782-7066db8e6b24",
          "name": "putScheduledUpdateGroupAction",
          "request": {
            "url": "http://example.com/api/?Action=PutScheduledUpdateGroupAction?AutoScalingGroupName=AutoScalingGroupName&DesiredCapacity=DesiredCapacity&EndTime=EndTime&MaxSize=MaxSize&MinSize=MinSize&Recurrence=Recurrence&ScheduledActionName=ScheduledActionName&StartTime=StartTime&Time=Time",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates or updates a scheduled scaling action for an Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9558f708-2964-43b8-ac7c-8884cc297ce9"
            }
          ]
        }
      ]
    },
    {
      "name": "Processes",
      "item": [
        {
          "id": "73265acd-5e6a-412e-89c4-a18daa1a61ce",
          "name": "resumeProcesses",
          "request": {
            "url": "http://example.com/api/?Action=ResumeProcesses?AutoScalingGroupName=AutoScalingGroupName&ScalingProcesses.member.N=ScalingProcesses.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Resumes the specified suspended Auto Scaling processes, or all suspended process, for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dac749fd-bc18-460b-8091-b910a9bbfced"
            }
          ]
        },
        {
          "id": "c529ab63-cea8-48ba-a8d9-7f6d865b5f30",
          "name": "suspendProcesses",
          "request": {
            "url": "http://example.com/api/?Action=SuspendProcesses?AutoScalingGroupName=AutoScalingGroupName&ScalingProcesses.member.N=ScalingProcesses.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Suspends the specified Auto Scaling processes, or all processes, for the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84b513cf-f1d5-4ddf-9822-51292c7c4b1a"
            }
          ]
        }
      ]
    },
    {
      "name": "Desired Capacity",
      "item": [
        {
          "id": "9e408a20-2dc3-4757-8b1f-5177ad1e4596",
          "name": "setDesiredCapacity",
          "request": {
            "url": "http://example.com/api/?Action=SetDesiredCapacity?AutoScalingGroupName=AutoScalingGroupName&DesiredCapacity=DesiredCapacity&HonorCooldown=HonorCooldown",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the size of the specified Auto Scaling group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5dff60a2-287f-44c2-845d-74136e276d50"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance Health",
      "item": [
        {
          "id": "b147dcfc-4ebb-469b-ba7b-e60157c3e3e7",
          "name": "setInstanceHealth",
          "request": {
            "url": "http://example.com/api/?Action=SetInstanceHealth?HealthStatus=HealthStatus&InstanceId=InstanceId&ShouldRespectGracePeriod=ShouldRespectGracePeriod",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the health status of the specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65472887-cbb1-47e9-9a71-5a431237bbdc"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance Protection",
      "item": [
        {
          "id": "e4b53f46-b84a-4c0b-9033-af6906d64e5f",
          "name": "setInstanceProtection",
          "request": {
            "url": "http://example.com/api/?Action=SetInstanceProtection?AutoScalingGroupName=AutoScalingGroupName&InstanceIds.member.N=InstanceIds.member.N&ProtectedFromScaleIn=ProtectedFromScaleIn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the instance protection settings of the specified instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b20b93ee-62ba-4552-8140-99ad68fbd9e4"
            }
          ]
        }
      ]
    }
  ]
}