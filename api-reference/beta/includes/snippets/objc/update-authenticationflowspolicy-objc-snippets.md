---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f1b5cac9dc5c3aea69895b567b96f212888235ccdd50e1e90b65f6595bb02aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902879"
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