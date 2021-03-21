---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d70e82fa23fe985cad4b7218cbb71763a4b7359c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959229"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/authentication/fido2Methods/-2_GRUg2-HYz6_1YG4YRAQ2"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphFido2AuthenticationMethod *fido2AuthenticationMethod = [[MSGraphFido2AuthenticationMethod alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```