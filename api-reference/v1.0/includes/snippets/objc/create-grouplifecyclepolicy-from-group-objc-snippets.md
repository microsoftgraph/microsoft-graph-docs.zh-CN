---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b3d618c7bf62850ddb9ce00b5f1c4b4403d6beb4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509716"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groupLifecyclePolicies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphGroupLifecyclePolicy *groupLifecyclePolicy = [[MSGraphGroupLifecyclePolicy alloc] init];
[groupLifecyclePolicy setGroupLifetimeInDays: 100];
[groupLifecyclePolicy setManagedGroupTypes:@"Selected"];
[groupLifecyclePolicy setAlternateNotificationEmails:@"admin@contoso.com"];

NSError *error;
NSData *groupLifecyclePolicyData = [groupLifecyclePolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:groupLifecyclePolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```