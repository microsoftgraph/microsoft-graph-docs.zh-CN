---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c809556dd50cd96feb2b7c0c8dbd6f83a7257b2
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458043"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/b2cAuthenticationMethodsPolicy"]]];
[urlRequest setHTTPMethod:@"PATCH"];

MSGraphB2cAuthenticationMethodsPolicy *b2cAuthenticationMethodsPolicy = [[MSGraphB2cAuthenticationMethodsPolicy alloc] init];
[b2cAuthenticationMethodsPolicy setIsEmailPasswordAuthenticationEnabled: false];
[b2cAuthenticationMethodsPolicy setIsUserNameAuthenticationEnabled: true];

NSError *error;
NSData *b2cAuthenticationMethodsPolicyData = [b2cAuthenticationMethodsPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:b2cAuthenticationMethodsPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```