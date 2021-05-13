---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e70273da36e3182d3d5ad972882d1640efa67f8
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475494"
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