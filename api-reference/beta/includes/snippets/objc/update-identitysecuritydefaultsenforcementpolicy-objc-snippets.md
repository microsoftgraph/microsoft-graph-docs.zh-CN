---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0727e7c896c2e66875b5d9130c4bdd76c14939ff
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947000"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/identitySecurityDefaultsEnforcementPolicy"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentitySecurityDefaultsEnforcementPolicy *identitySecurityDefaultsEnforcementPolicy = [[MSGraphIdentitySecurityDefaultsEnforcementPolicy alloc] init];
[identitySecurityDefaultsEnforcementPolicy setIsEnabled: false];

NSError *error;
NSData *identitySecurityDefaultsEnforcementPolicyData = [identitySecurityDefaultsEnforcementPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:identitySecurityDefaultsEnforcementPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```