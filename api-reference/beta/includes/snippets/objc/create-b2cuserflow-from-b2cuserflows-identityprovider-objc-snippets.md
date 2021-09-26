---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 032a97a9e81a584652e308182148f798e7f489a4
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763499"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2cUserFlows"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"https://graph.microsoft.com/beta/identity/b2cUserFlows('B2C_1_Customer')" forHTTPHeaderField:@"Location"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphB2cIdentityUserFlow *b2cIdentityUserFlow = [[MSGraphB2cIdentityUserFlow alloc] init];
[b2cIdentityUserFlow setId:@"Customer"];
[b2cIdentityUserFlow setUserFlowType: [MSGraphUserFlowType signUpOrSignIn]];
[b2cIdentityUserFlow setUserFlowTypeVersion: 3];
NSMutableArray *identityProvidersList = [[NSMutableArray alloc] init];
MSGraphIdentityProvider *identityProviders = [[MSGraphIdentityProvider alloc] init];
[identityProviders setId:@"Facebook-OAuth"];
[identityProvidersList addObject: identityProviders];
[b2cIdentityUserFlow setIdentityProviders:identityProvidersList];

NSError *error;
NSData *b2cIdentityUserFlowData = [b2cIdentityUserFlow getSerializedDataWithError:&error];
[urlRequest setHTTPBody:b2cIdentityUserFlowData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```