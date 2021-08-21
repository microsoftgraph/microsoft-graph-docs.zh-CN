---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cb1268690ee9bd16489b97a30ef65d6d82e26c38dbc44eb0f251d325f994418
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105804"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedAccess/azureResources/roleAssignmentRequests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphGovernanceRoleAssignmentRequest *governanceRoleAssignmentRequest = [[MSGraphGovernanceRoleAssignmentRequest alloc] init];
[governanceRoleAssignmentRequest setRoleDefinitionId:@"bc75b4e6-7403-4243-bf2f-d1f6990be122"];
[governanceRoleAssignmentRequest setResourceId:@"fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735"];
[governanceRoleAssignmentRequest setSubjectId:@"918e54be-12c4-4f4c-a6d3-2ee0e3661c51"];
[governanceRoleAssignmentRequest setAssignmentState:@"Active"];
[governanceRoleAssignmentRequest setType:@"UserRemove"];
[governanceRoleAssignmentRequest setReason:@"Deactivate the role"];
[governanceRoleAssignmentRequest setLinkedEligibleRoleAssignmentId:@"cb8a533e-02d5-42ad-8499-916b1e4822ec"];

NSError *error;
NSData *governanceRoleAssignmentRequestData = [governanceRoleAssignmentRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:governanceRoleAssignmentRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```