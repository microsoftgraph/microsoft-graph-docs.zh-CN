---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0e5d40b4ef51dc5ce389a72823b1dbe1dd6bba0
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869080"
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