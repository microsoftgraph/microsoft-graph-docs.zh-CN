---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6def7b5a37432a1f1de0ed1db9ce5a3bc75b5efbc7489653138a8e65bc3e29e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162226"
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