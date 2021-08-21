---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0716e8d3d8721f41cdfa3971ba80aecbd96bdcf55da8a88e94c0ef2bce1b9c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903606"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleAssignmentScheduleRequests/"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUnifiedRoleAssignmentScheduleRequest *unifiedRoleAssignmentScheduleRequest = [[MSGraphUnifiedRoleAssignmentScheduleRequest alloc] init];
[unifiedRoleAssignmentScheduleRequest setAction:@"String"];
[unifiedRoleAssignmentScheduleRequest setPrincipalId:@"String"];
[unifiedRoleAssignmentScheduleRequest setRoleDefinitionId:@"String"];
[unifiedRoleAssignmentScheduleRequest setDirectoryScopeId:@"String"];
[unifiedRoleAssignmentScheduleRequest setAppScopeId:@"String"];
[unifiedRoleAssignmentScheduleRequest setIsValidationOnly:@"Boolean"];
[unifiedRoleAssignmentScheduleRequest setTargetScheduleId:@"String"];
[unifiedRoleAssignmentScheduleRequest setJustification:@"String"];
MSGraphRequestSchedule *scheduleInfo = [[MSGraphRequestSchedule alloc] init];
[unifiedRoleAssignmentScheduleRequest setScheduleInfo:scheduleInfo];
MSGraphTicketInfo *ticketInfo = [[MSGraphTicketInfo alloc] init];
[unifiedRoleAssignmentScheduleRequest setTicketInfo:ticketInfo];

NSError *error;
NSData *unifiedRoleAssignmentScheduleRequestData = [unifiedRoleAssignmentScheduleRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:unifiedRoleAssignmentScheduleRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```