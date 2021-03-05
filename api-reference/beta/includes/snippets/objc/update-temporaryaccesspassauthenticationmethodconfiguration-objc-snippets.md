---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7546492b16a850a352af1d1b1a524a9e9ed45904
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471855"
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