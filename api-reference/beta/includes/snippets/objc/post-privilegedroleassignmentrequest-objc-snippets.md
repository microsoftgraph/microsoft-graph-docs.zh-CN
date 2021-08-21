---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a00ecbc5fc4f5d81747f638540888d035b844b8d87f0fcbc576b2043ff338382
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163211"
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