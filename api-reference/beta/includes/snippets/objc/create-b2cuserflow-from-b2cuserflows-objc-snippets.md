---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c9b5f07bb4f1e39e9519b1abefbf7bcd8bda78bee2d04ba7122476d0ca0db30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161468"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2cUserFlows"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphB2cIdentityUserFlow *b2cIdentityUserFlow = [[MSGraphB2cIdentityUserFlow alloc] init];
[b2cIdentityUserFlow setId:@"Customer"];
[b2cIdentityUserFlow setUserFlowType: [MSGraphUserFlowType signUpOrSignIn]];
[b2cIdentityUserFlow setUserFlowTypeVersion: 3];

NSError *error;
NSData *b2cIdentityUserFlowData = [b2cIdentityUserFlow getSerializedDataWithError:&error];
[urlRequest setHTTPBody:b2cIdentityUserFlowData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```