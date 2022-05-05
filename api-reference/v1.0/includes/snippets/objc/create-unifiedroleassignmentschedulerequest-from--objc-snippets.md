---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfd27875d481df7aa6f92b1a0be33f2f8daab686
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206770"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleAssignmentScheduleRequests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUnifiedRoleAssignmentScheduleRequest *unifiedRoleAssignmentScheduleRequest = [[MSGraphUnifiedRoleAssignmentScheduleRequest alloc] init];
[unifiedRoleAssignmentScheduleRequest setAction: [MSGraphUnifiedRoleScheduleRequestActions adminAssign]];
[unifiedRoleAssignmentScheduleRequest setJustification:@"Assign Groups Admin to IT Helpdesk group"];
[unifiedRoleAssignmentScheduleRequest setRoleDefinitionId:@"fdd7a751-b60b-444a-984c-02652fe8fa1c"];
[unifiedRoleAssignmentScheduleRequest setDirectoryScopeId:@"/"];
[unifiedRoleAssignmentScheduleRequest setPrincipalId:@"071cc716-8147-4397-a5ba-b2105951cc0b"];
MSGraphRequestSchedule *scheduleInfo = [[MSGraphRequestSchedule alloc] init];
[scheduleInfo setStartDateTime: "2022-04-10T00:00:00Z"];
MSGraphExpirationPattern *expiration = [[MSGraphExpirationPattern alloc] init];
[expiration setType: [MSGraphExpirationPatternType noExpiration]];
[scheduleInfo setExpiration:expiration];
[unifiedRoleAssignmentScheduleRequest setScheduleInfo:scheduleInfo];

NSError *error;
NSData *unifiedRoleAssignmentScheduleRequestData = [unifiedRoleAssignmentScheduleRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:unifiedRoleAssignmentScheduleRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```