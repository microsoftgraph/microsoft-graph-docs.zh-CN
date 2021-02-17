---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 013cf797c26c49566d5399782edcd9f8767b8fe8
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272439"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/rosters/6519868f-868f-6519-8f86-19658f861965/members"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPlannerRosterMember *plannerRosterMember = [[MSGraphPlannerRosterMember alloc] init];
[plannerRosterMember setUserId:@"String"];

NSError *error;
NSData *plannerRosterMemberData = [plannerRosterMember getSerializedDataWithError:&error];
[urlRequest setHTTPBody:plannerRosterMemberData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```