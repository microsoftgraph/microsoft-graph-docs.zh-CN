---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a67e635be952acaa0554088aa42b104c162fa5717bb3995b82a22d1a312ddf9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378376"
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