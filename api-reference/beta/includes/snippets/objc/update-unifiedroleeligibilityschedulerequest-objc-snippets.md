---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6acd70ed4901917dcdc6626904066eb2c35da3e7
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474379"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
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