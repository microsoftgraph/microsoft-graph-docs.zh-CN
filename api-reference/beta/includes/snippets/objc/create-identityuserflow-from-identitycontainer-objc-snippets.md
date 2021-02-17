---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1faf826b15278a0f3d6f2c6d2ed7048544d26e9f
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274790"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/userFlows"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityUserFlow *identityUserFlow = [[MSGraphIdentityUserFlow alloc] init];
[identityUserFlow setId:@"Pol1"];
[identityUserFlow setUserFlowType: [MSGraphUserFlowType signUpOrSignIn]];
[identityUserFlow setUserFlowTypeVersion: 1];

NSError *error;
NSData *identityUserFlowData = [identityUserFlow getSerializedDataWithError:&error];
[urlRequest setHTTPBody:identityUserFlowData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```