---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8235c853ddcd09fda47b70d0e901ee0fb38a507
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580833"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/authenticationMethodsPolicy"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAuthenticationMethodsPolicy *authenticationMethodsPolicy = [[MSGraphAuthenticationMethodsPolicy alloc] init];
NSMutableArray *authenticationMethodConfigurationsList = [[NSMutableArray alloc] init];
MSGraphAuthenticationMethodConfiguration *authenticationMethodConfigurations = [[MSGraphAuthenticationMethodConfiguration alloc] init];
[authenticationMethodConfigurations setId:@"Fido2"];
[authenticationMethodConfigurations setState: [MSGraphAuthenticationMethodState disabled]];
[authenticationMethodConfigurations setIsSelfServiceRegistrationAllowed: false];
[authenticationMethodConfigurations setIsAttestationEnforced: false];
MSGraphFido2KeyRestrictions *keyRestrictions = [[MSGraphFido2KeyRestrictions alloc] init];
[keyRestrictions setIsEnforced: false];
[keyRestrictions setEnforcementType: [MSGraphFido2RestrictionEnforcementType block]];
NSMutableArray *aaGuidsList = [[NSMutableArray alloc] init];
[keyRestrictions setAaGuids:aaGuidsList];
[authenticationMethodConfigurations setKeyRestrictions:keyRestrictions];
[authenticationMethodConfigurationsList addObject: authenticationMethodConfigurations];
[authenticationMethodsPolicy setAuthenticationMethodConfigurations:authenticationMethodConfigurationsList];

NSError *error;
NSData *authenticationMethodsPolicyData = [authenticationMethodsPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:authenticationMethodsPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```