---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c783b397c1cb8afeff93433b6e33e875b6fa71ba813c37e1c552de865bbfcbf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161759"
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