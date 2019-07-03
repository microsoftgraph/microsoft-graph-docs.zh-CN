---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9e00f996d68618f55690418f328771e84ab30335
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479481"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedRoleAssignmentRequests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPrivilegedRoleAssignmentRequest *privilegedRoleAssignmentRequest = [[MSGraphPrivilegedRoleAssignmentRequest alloc] init];
[privilegedRoleAssignmentRequest setDuration:@"2"];
[privilegedRoleAssignmentRequest setReason:@"Activate the role for business purpose"];
[privilegedRoleAssignmentRequest setTicketNumber:@"234"];
[privilegedRoleAssignmentRequest setTicketSystem:@"system"];
MSGraphGovernanceSchedule *schedule = [[MSGraphGovernanceSchedule alloc] init];
[schedule setStartDateTime: "2018-02-08T02:35:17.903Z"];
[privilegedRoleAssignmentRequest setSchedule:schedule];
[privilegedRoleAssignmentRequest setEvaluateOnly: false];
[privilegedRoleAssignmentRequest setType:@"UserAdd"];
[privilegedRoleAssignmentRequest setAssignmentState:@"Active"];
[privilegedRoleAssignmentRequest setRoleId:@"88d8e3e3-8f55-4a1e-953a-9b9898b8876b"];

NSError *error;
NSData *privilegedRoleAssignmentRequestData = [privilegedRoleAssignmentRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:privilegedRoleAssignmentRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```