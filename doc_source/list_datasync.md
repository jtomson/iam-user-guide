# Actions, resources, and condition keys for DataSync<a name="list_datasync"></a>

**Tip**  
This page is moving to a new location on November 16, 2020\. Please update your bookmark to use the new page at [https://docs\.aws\.amazon\.com/service\-authorization/latest/reference/list\_datasync\.html](https://docs.aws.amazon.com/service-authorization/latest/reference/list_datasync.html)\. 

DataSync \(service prefix: `datasync`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/datasync/latest/userguide/)\.
+ View a list of the [API operations available for this service](https://docs.aws.amazon.com/datasync/latest/userguide/API_Reference.html)\.
+ Learn how to secure this service and its resources by [using IAM](https://docs.aws.amazon.com/datasync/latest/userguide/iam.html) permission policies\.

**Topics**
+ [Actions defined by DataSync](#datasync-actions-as-permissions)
+ [Resource types defined by DataSync](#datasync-resources-for-iam-policies)
+ [Condition keys for DataSync](#datasync-policy-keys)

## Actions defined by DataSync<a name="datasync-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. Use policies to grant permissions to perform an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\.

The **Resource types** column indicates whether each action supports resource\-level permissions\. If there is no value for this column, you must specify all resources \("\*"\) in the `Resource` element of your policy statement\. If the column includes a resource type, then you can specify an ARN of that type in a statement with that action\. Required resources are indicated in the table with an asterisk \(\*\)\. If you specify a resource\-level permission ARN in a statement using this action, then it must be of this type\. Some actions support multiple resource types\. If the resource type is optional \(not indicated as required\), then you can choose to use one but not the other\.

For details about the columns in the following table, see [The actions table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  
[\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/IAM/latest/UserGuide/list_datasync.html)

## Resource types defined by DataSync<a name="datasync-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#datasync-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The resource types table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource types | ARN | Condition keys | 
| --- | --- | --- | 
|   [ agent ](https://docs.aws.amazon.com/datasync/latest/userguide/agent.html)  |  arn:$\{Partition\}:datasync:$\{Region\}:$\{AccountId\}:agent/$\{AgentId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#datasync-aws_ResourceTag___TagKey_)   | 
|   [ location ](https://docs.aws.amazon.com/datasync/latest/userguide/location.html)  |  arn:$\{Partition\}:datasync:$\{Region\}:$\{AccountId\}:location/$\{LocationId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#datasync-aws_ResourceTag___TagKey_)   | 
|   [ task ](https://docs.aws.amazon.com/datasync/latest/userguide/task.html)  |  arn:$\{Partition\}:datasync:$\{Region\}:$\{AccountId\}:task/$\{TaskId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#datasync-aws_ResourceTag___TagKey_)   | 
|   [ taskexecution ](https://docs.aws.amazon.com/datasync/latest/userguide/taskexecution.html)  |  arn:$\{Partition\}:datasync:$\{Region\}:$\{AccountId\}:task/$\{TaskId\}/execution/$\{ExecutionId\}  |  | 

## Condition keys for DataSync<a name="datasync-policy-keys"></a>

DataSync defines the following condition keys that can be used in the `Condition` element of an IAM policy\. You can use these keys to further refine the conditions under which the policy statement applies\. For details about the columns in the following table, see [The condition keys table](reference_policies_actions-resources-contextkeys.md#context_keys_table)\.

To view the global condition keys that are available to all services, see [Available global condition keys](reference_policies_condition-keys.html#AvailableKeys)\.


****  

| Condition keys | Description | Type | 
| --- | --- | --- | 
|   aws:RequestTag/$\{TagKey\}  | Filters create requests based on the allowed set of values for each of the tags\. | String | 
|   aws:ResourceTag/$\{TagKey\}  | Filters actions based on tag\-value associated with the resource\. | String | 
|   aws:TagKeys  | Filters create requests based on the presence of mandatory tags in the request\. | String | 