---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b808256cfd4105706470c64947dd34b618e20d172354c0dca90663f61590425
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158353"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/TemporaryAccessPass"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAuthenticationMethodConfiguration *authenticationMethodConfiguration = [[MSGraphAuthenticationMethodConfiguration alloc] init];
[authenticationMethodConfiguration setState: [MSGraphAuthenticationMethodState enabled]];
[authenticationMethodConfiguration setDefaultLifetimeInMinutes: 60];
[authenticationMethodConfiguration setDefaultLength: 8];
[authenticationMethodConfiguration setMinimumLifetimeInMinutes: 60];
[authenticationMethodConfiguration setMaximumLifetimeInMinutes: 1440];
[authenticationMethodConfiguration set
  isUsableOnce: false];
NSMutableArray *includeTargetsList = [[NSMutableArray alloc] init];
MSGraphAuthenticationMethodTarget *includeTargets = [[MSGraphAuthenticationMethodTarget alloc] init];
[includeTargets setTargetType: [MSGraphAuthenticationMethodTargetType group]];
[includeTargets setId:@"all_users"];
[includeTargets setIsRegistrationRequired: false];
[includeTargets setUseForSignIn: true];
[includeTargetsList addObject: includeTargets];
[authenticationMethodConfiguration setIncludeTargets:includeTargetsList];

NSError *error;
NSData *authenticationMethodConfigurationData = [authenticationMethodConfiguration getSerializedDataWithError:&error];
[urlRequest setHTTPBody:authenticationMethodConfigurationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```