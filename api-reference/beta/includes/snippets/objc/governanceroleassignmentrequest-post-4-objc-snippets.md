---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ccfb1897a4d1bb2ed4ae09a4258330fa47c93869
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950791"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedAccess/azureResources/roleAssignmentRequests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphGovernanceRoleAssignmentRequest *governanceRoleAssignmentRequest = [[MSGraphGovernanceRoleAssignmentRequest alloc] init];
[governanceRoleAssignmentRequest setRoleDefinitionId:@"65bb4622-61f5-4f25-9d75-d0e20cf92019"];
[governanceRoleAssignmentRequest setResourceId:@"e5e7d29d-5465-45ac-885f-4716a5ee74b5"];
[governanceRoleAssignmentRequest setSubjectId:@"74765671-9ca4-40d7-9e36-2f4a570608a6"];
[governanceRoleAssignmentRequest setAssignmentState:@"Eligible"];
[governanceRoleAssignmentRequest setType:@"AdminRemove"];

NSError *error;
NSData *governanceRoleAssignmentRequestData = [governanceRoleAssignmentRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:governanceRoleAssignmentRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```