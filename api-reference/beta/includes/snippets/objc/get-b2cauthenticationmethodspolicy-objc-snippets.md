---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec4f45c033724285861c20956f16d6e9015a1200b1a384d6ed1a5f9936c81e2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105285"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/b2cAuthenticationMethodsPolicy"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphB2cAuthenticationMethodsPolicy *b2cAuthenticationMethodsPolicy = [[MSGraphB2cAuthenticationMethodsPolicy alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```