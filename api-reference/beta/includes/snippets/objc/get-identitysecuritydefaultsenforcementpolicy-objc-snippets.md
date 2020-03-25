---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0515506339a69870dddd7abb86426a5535926481
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947057"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/identitySecurityDefaultsEnforcementPolicy"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphIdentitySecurityDefaultsEnforcementPolicy *identitySecurityDefaultsEnforcementPolicy = [[MSGraphIdentitySecurityDefaultsEnforcementPolicy alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```