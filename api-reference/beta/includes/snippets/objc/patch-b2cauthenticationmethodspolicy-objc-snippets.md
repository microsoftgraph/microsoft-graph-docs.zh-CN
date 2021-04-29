---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 125d7209014fecedf27f406a10ff24ff2243469a
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52081500"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/b2cAuthenticationMethodsPolicy"]]];
[urlRequest setHTTPMethod:@"PATCH"];

MSGraphB2cAuthenticationMethodsPolicy *b2cAuthenticationMethodsPolicy = [[MSGraphB2cAuthenticationMethodsPolicy alloc] init];
[b2cAuthenticationMethodsPolicy setIsEmailPasswordAuthenticationEnabled: false];
[b2cAuthenticationMethodsPolicy setIsUserNameAuthenticationEnabled: true];
[b2cAuthenticationMethodsPolicy setIsPhoneOneTimePasswordAuthenticationEnabled: true];

NSError *error;
NSData *b2cAuthenticationMethodsPolicyData = [b2cAuthenticationMethodsPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:b2cAuthenticationMethodsPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```