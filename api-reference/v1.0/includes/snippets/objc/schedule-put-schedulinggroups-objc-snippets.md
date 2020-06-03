---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad28eeac96e2f50e8145baa1a24b3ac15ef14c63
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44215841"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"return=representation" forHTTPHeaderField:@"Prefer"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSchedulingGroup *schedulingGroup = [[MSGraphSchedulingGroup alloc] init];
[schedulingGroup setDisplayName:@"Cashiers"];
[schedulingGroup setIsActive: true];
NSMutableArray *userIdsList = [[NSMutableArray alloc] init];
[userIdsList addObject: @"c5d0c76b-80c4-481c-be50-923cd8d680a1"];
[userIdsList addObject: @"2a4296b3-a28a-44ba-bc66-0274b9b95851"];
[schedulingGroup setUserIds:userIdsList];

NSError *error;
NSData *schedulingGroupData = [schedulingGroup getSerializedDataWithError:&error];
[urlRequest setHTTPBody:schedulingGroupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```