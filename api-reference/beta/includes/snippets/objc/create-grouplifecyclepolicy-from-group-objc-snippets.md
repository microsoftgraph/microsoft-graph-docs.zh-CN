---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2346712a60c8b5ec863caf68858634278ca48849
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612354"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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