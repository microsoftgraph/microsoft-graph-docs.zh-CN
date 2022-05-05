---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86ce28c268f22864856c558db6c099edebdfe186
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206799"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleAssignmentScheduleRequests/"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUnifiedRoleAssignmentScheduleRequest *unifiedRoleAssignmentScheduleRequest = [[MSGraphUnifiedRoleAssignmentScheduleRequest alloc] init];
[unifiedRoleAssignmentScheduleRequest setAction: [MSGraphUnifiedRoleScheduleRequestActions selfActivate]];
[unifiedRoleAssignmentScheduleRequest setPrincipalId:@"071cc716-8147-4397-a5ba-b2105951cc0b"];
[unifiedRoleAssignmentScheduleRequest setRoleDefinitionId:@"8424c6f0-a189-499e-bbd0-26c1753c96d4"];
[unifiedRoleAssignmentScheduleRequest setDirectoryScopeId:@"/"];
[unifiedRoleAssignmentScheduleRequest setJustification:@"I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs"];
MSGraphRequestSchedule *scheduleInfo = [[MSGraphRequestSchedule alloc] init];
[scheduleInfo setStartDateTime: "2022-04-14T00:00:00Z"];
MSGraphExpirationPattern *expiration = [[MSGraphExpirationPattern alloc] init];
[expiration setType: [MSGraphExpirationPatternType afterDuration]];
[expiration setDuration:@"PT5H"];
[scheduleInfo setExpiration:expiration];
[unifiedRoleAssignmentScheduleRequest setScheduleInfo:scheduleInfo];
MSGraphTicketInfo *ticketInfo = [[MSGraphTicketInfo alloc] init];
[ticketInfo setTicketNumber:@"CONTOSO:Normal-67890"];
[ticketInfo setTicketSystem:@"MS Project"];
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