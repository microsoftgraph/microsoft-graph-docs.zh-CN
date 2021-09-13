---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f21f5f1d8795a35ef1f7cde4796b10a78741004acab0a17f5fc86b43c7c1fff9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106732"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/homeRealmDiscoveryPolicies/{id}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphHomeRealmDiscoveryPolicy *homeRealmDiscoveryPolicy = [[MSGraphHomeRealmDiscoveryPolicy alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```