---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 375fd4dc82b5c36a1866bf6faae016bb6e5491a52ac8ae445aa0e6708b7d756a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162130"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2xUserFlows/B2X_1_Test/userflowIdentityProviders/$ref"]]];
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