---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48af100ff13de874f348790075e019ce1732c37c11e9f5e31daaf46eb9d6a20c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333255"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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