---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cc510a8e99029568357a8c381eb9cfe3118b65477e0049d39f21d1ad9df1549
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218510"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *@odata.type = @"#microsoft.graph.cloudPcProvisioningPolicyAssignment";
payloadDictionary[@"@odata.type"] = @odata.type;

NSMutableArray *assignmentsList = [[NSMutableArray alloc] init];
MSGraphCloudPcProvisioningPolicyAssignment *assignments = [[MSGraphCloudPcProvisioningPolicyAssignment alloc] init];
[assignments setId:@"b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff"];
MSGraphCloudPcManagementAssignmentTarget *target = [[MSGraphCloudPcManagementAssignmentTarget alloc] init];
[target setGroupId:@"64ff06de-9c00-4a5a-98b5-7f5abe26ffff"];
[assignments setTarget:target];
[assignmentsList addObject: assignments];
payloadDictionary[@"assignments"] = assignmentsList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```