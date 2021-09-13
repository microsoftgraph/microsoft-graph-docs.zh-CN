---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a4d38d7d953ec1fa85840540a65122b316f3ca5aac5203b26929f5d7a6861dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332976"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/identitySecurityDefaultsEnforcementPolicy"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphIdentitySecurityDefaultsEnforcementPolicy *identitySecurityDefaultsEnforcementPolicy = [[MSGraphIdentitySecurityDefaultsEnforcementPolicy alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```