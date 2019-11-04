---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 460714767933e2c2a4b50773a3b988c873f0effb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938558"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/userFlows"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityUserFlow *identityUserFlow = [[MSGraphIdentityUserFlow alloc] init];
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