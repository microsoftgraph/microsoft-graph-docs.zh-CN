---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 900c2327e670f1773465399b3c7756121f7e73725db7835abd3431f8d66b9d48
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332580"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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