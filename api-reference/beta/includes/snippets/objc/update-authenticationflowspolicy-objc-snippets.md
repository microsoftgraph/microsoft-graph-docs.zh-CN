---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45c66d6bb8a24df7cc5786d993083374cc9971aa
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44680880"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/authenticationFlowsPolicy"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAuthenticationFlowsPolicy *authenticationFlowsPolicy = [[MSGraphAuthenticationFlowsPolicy alloc] init];
MSGraphSelfServiceSignUpAuthenticationFlowConfiguration *selfServiceSignUp = [[MSGraphSelfServiceSignUpAuthenticationFlowConfiguration alloc] init];
[selfServiceSignUp setIsEnabled: true];
[authenticationFlowsPolicy setSelfServiceSignUp:selfServiceSignUp];

NSError *error;
NSData *authenticationFlowsPolicyData = [authenticationFlowsPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:authenticationFlowsPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```