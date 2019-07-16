---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6ff6a33b69720d4c0dc1a4813c787311756f1283
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738357"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/subscriptions"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *subscriptionList = [[NSMutableArray alloc] init];
        subscriptionList = [jsonFinal valueForKey:@"value"];
        MSGraphSubscription *subscription = [[MSGraphSubscription alloc] initWithDictionary:[subscriptionList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```