---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 535eaf41b28152cde724696b25abaf5a145b90f0ff81c1ee8044591acbbdde8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105386"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/identityProviders"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityProviderBase *identityProviderBase = [[MSGraphIdentityProviderBase alloc] init];
[identityProviderBase setDisplayName:@"Login with Amazon"];
[identityProviderBase setIdentityProviderType:@"Amazon"];
[identityProviderBase setClientId:@"56433757-cadd-4135-8431-2c9e3fd68ae8"];
[identityProviderBase setClientSecret:@"000000000000"];

NSError *error;
NSData *identityProviderBaseData = [identityProviderBase getSerializedDataWithError:&error];
[urlRequest setHTTPBody:identityProviderBaseData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```