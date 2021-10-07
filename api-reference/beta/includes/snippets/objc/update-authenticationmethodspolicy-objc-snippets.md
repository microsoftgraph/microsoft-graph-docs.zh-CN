---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca66122b019ea152cd79c70fdbb63f82b05e5877ba2a3d2314663e4203622cfe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105666"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/authenticationMethodsPolicy"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAuthenticationMethodsPolicy *authenticationMethodsPolicy = [[MSGraphAuthenticationMethodsPolicy alloc] init];
MSGraphRegistrationEnforcement *registrationEnforcement = [[MSGraphRegistrationEnforcement alloc] init];
MSGraphAuthenticationMethodsRegistrationCampaign *authenticationMethodsRegistrationCampaign = [[MSGraphAuthenticationMethodsRegistrationCampaign alloc] init];
[authenticationMethodsRegistrationCampaign setSnoozeDurationInDays: 1];
[authenticationMethodsRegistrationCampaign setState: [MSGraphAdvancedConfigState enabled]];
NSMutableArray *excludeTargetsList = [[NSMutableArray alloc] init];
[authenticationMethodsRegistrationCampaign setExcludeTargets:excludeTargetsList];
NSMutableArray *includeTargetsList = [[NSMutableArray alloc] init];
MSGraphAuthenticationMethodsRegistrationCampaignIncludeTarget *includeTargets = [[MSGraphAuthenticationMethodsRegistrationCampaignIncludeTarget alloc] init];
[includeTargets setId:@"3ee3a9de-0a86-4e12-a287-9769accf1ba2"];
[includeTargets setTargetType: [MSGraphAuthenticationMethodTargetType group]];
[includeTargets setTargetedAuthenticationMethod:@"microsoftAuthenticator"];
[includeTargetsList addObject: includeTargets];
[authenticationMethodsRegistrationCampaign setIncludeTargets:includeTargetsList];
[registrationEnforcement setAuthenticationMethodsRegistrationCampaign:authenticationMethodsRegistrationCampaign];
[authenticationMethodsPolicy setRegistrationEnforcement:registrationEnforcement];

NSError *error;
NSData *authenticationMethodsPolicyData = [authenticationMethodsPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:authenticationMethodsPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```