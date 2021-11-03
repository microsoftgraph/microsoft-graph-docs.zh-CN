---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2776f78dc65cf2517f6e756c1aa3f340b3236d37
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60690181"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/applications/acd7c908-1c4d-4d48-93ee-ff38349a75c8/federatedIdentityCredentials/bdad0963-4a7a-43ae-b569-e67e1da3f2c0"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphFederatedIdentityCredential *federatedIdentityCredential = [[MSGraphFederatedIdentityCredential alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```