<!--
Copyright 2015-2017 Amazon.com, Inc. or its affiliates. All Rights Reserved.

Licensed under the Apache License, Version 2.0 (the "License"). You may
not use this file except in compliance with the License. A copy of the
License is located at

http://aws.amazon.com/apache2.0/

or in the "license" file accompanying this file. This file is distributed
on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
express or implied. See the License for the specific language governing
permissions and limitations under the License.
-->

#Support ECS autoscaling in compose

##Introduction
([#Issue 205](https://github.com/aws/amazon-ecs-cli/issues/205))

The current implementation of ecs-cli does not support autoscaling of the service after it has been setup.

##Resources that is involved

AWS::AutoScaling::ScalingPolicy

https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-as-policy.html

AWS::ApplicationAutoScaling::ScalableTarget

https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-applicationautoscaling-scalabletarget.html

AWS::CloudWatch::Alarm

https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-cw-alarm.html


##Proposal
