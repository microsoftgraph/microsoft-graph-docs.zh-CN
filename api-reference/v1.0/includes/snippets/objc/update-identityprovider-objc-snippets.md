---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cd2518bb6b76dab7e59bb33a4d19cfb674da1b10
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731582"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityProviders/Amazon-OAuth"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityProvider *identityProvider = [[MSGraphIdentityProvider alloc] init];
[identityProvider setClientSecret:@"1111111111111"];

NSError *error;
NSData *identityProviderData = [identityProvider getSerializedDataWithError:&error];
[urlRequest setHTTPBody:identityProviderData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```