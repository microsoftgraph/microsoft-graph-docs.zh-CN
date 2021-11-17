---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e57bed6a91c7c4973f5a2abdd47128ef9703786bc00c235b7f4ae8009aa5ac3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162207"
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