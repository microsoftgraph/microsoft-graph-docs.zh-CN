---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d3ed2ce91f9fa19bb0453dda7f48a10404dd4ccf736577487b1bfc02c8114d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162481"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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