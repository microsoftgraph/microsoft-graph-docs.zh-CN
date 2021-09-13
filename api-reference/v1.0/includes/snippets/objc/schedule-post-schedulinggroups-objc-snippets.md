---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd5fb1192f7e7208e5ba8d4c0f0094defc0b6aa8df94dd9100448fe6a380c88e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161781"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{teamId}/schedule/schedulingGroups"]]];
[urlRequest setHTTPMethod:@"POST"];
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