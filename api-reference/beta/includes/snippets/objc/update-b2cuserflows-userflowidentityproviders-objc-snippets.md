---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7d3b3764be0b0ea1d47059e72905cdc3c058e3c
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439706"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders/$ref"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityProviderBase *userFlowIdentityProviders = [[MSGraphIdentityProviderBase alloc] init];

NSError *error;
NSData *userFlowIdentityProvidersData = [userFlowIdentityProviders getSerializedDataWithError:&error];
[urlRequest setHTTPBody:userFlowIdentityProvidersData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```