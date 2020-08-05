---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71928c5038da8901dddf0024c74cdb4bf605ca8b
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46570120"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphRiskyUserHistoryItem *riskyUserHistoryItem = [[MSGraphRiskyUserHistoryItem alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```