---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59b3baa7a8c978290d47cb974dd41e7c11807ca7
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211230"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals?$filter=startswith(displayName,%20'a')&$count=true&$top=1&$orderby=displayName"]]];
[urlRequest setHTTPMethod:@"GET"];
[urlRequest setValue:@"eventual" forHTTPHeaderField:@"ConsistencyLevel"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphServicePrincipal *servicePrincipal = [[MSGraphServicePrincipal alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```