---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 305788db302fe06bedd9ee555a2f57d19ce33480
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513958"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleEligibilityScheduleRequests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUnifiedRoleEligibilityScheduleRequest *unifiedRoleEligibilityScheduleRequest = [[MSGraphUnifiedRoleEligibilityScheduleRequest alloc] init];
[unifiedRoleEligibilityScheduleRequest setAction:@"AdminRemove"];
[unifiedRoleEligibilityScheduleRequest setJustification:@"Assign User Admin eligibility to IT Helpdesk (User) group"];
[unifiedRoleEligibilityScheduleRequest setRoleDefinitionId:@"fdd7a751-b60b-444a-984c-02652fe8fa1c"];
[unifiedRoleEligibilityScheduleRequest setDirectoryScopeId:@"/"];
[unifiedRoleEligibilityScheduleRequest setPrincipalId:@"07706ff1-46c7-4847-ae33-3003830675a1"];
MSGraphRequestSchedule *scheduleInfo = [[MSGraphRequestSchedule alloc] init];
[scheduleInfo setStartDateTime: "2021-07-26T18:08:06.2081758Z"];
MSGraphExpirationPattern *expiration = [[MSGraphExpirationPattern alloc] init];
[expiration setEndDateTime: "2022-06-30T00:00:00Z"];
[expiration setType: [MSGraphExpirationPatternType afterDateTime]];
[scheduleInfo setExpiration:expiration];
[unifiedRoleEligibilityScheduleRequest setScheduleInfo:scheduleInfo];

NSError *error;
NSData *unifiedRoleEligibilityScheduleRequestData = [unifiedRoleEligibilityScheduleRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:unifiedRoleEligibilityScheduleRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```