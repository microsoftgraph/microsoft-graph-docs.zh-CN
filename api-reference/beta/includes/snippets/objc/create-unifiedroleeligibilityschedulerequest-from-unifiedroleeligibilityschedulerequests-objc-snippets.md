---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: feb7d9737895610c6634b7b2516a6a8062a1b36b
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475204"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleEligibilityScheduleRequests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUnifiedRoleEligibilityScheduleRequest *unifiedRoleEligibilityScheduleRequest = [[MSGraphUnifiedRoleEligibilityScheduleRequest alloc] init];
[unifiedRoleEligibilityScheduleRequest setAction:@"String"];
[unifiedRoleEligibilityScheduleRequest setPrincipalId:@"String"];
[unifiedRoleEligibilityScheduleRequest setRoleDefinitionId:@"String"];
[unifiedRoleEligibilityScheduleRequest setDirectoryScopeId:@"String"];
[unifiedRoleEligibilityScheduleRequest setAppScopeId:@"String"];
[unifiedRoleEligibilityScheduleRequest setIsValidationOnly:@"Boolean"];
[unifiedRoleEligibilityScheduleRequest setTargetScheduleId:@"String"];
[unifiedRoleEligibilityScheduleRequest setJustification:@"String"];
MSGraphRequestSchedule *scheduleInfo = [[MSGraphRequestSchedule alloc] init];
[unifiedRoleEligibilityScheduleRequest setScheduleInfo:scheduleInfo];
MSGraphTicketInfo *ticketInfo = [[MSGraphTicketInfo alloc] init];
[unifiedRoleEligibilityScheduleRequest setTicketInfo:ticketInfo];

NSError *error;
NSData *unifiedRoleEligibilityScheduleRequestData = [unifiedRoleEligibilityScheduleRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:unifiedRoleEligibilityScheduleRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```