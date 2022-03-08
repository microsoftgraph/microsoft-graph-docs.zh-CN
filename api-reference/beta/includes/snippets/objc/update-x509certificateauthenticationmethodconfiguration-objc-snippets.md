---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9011f0d41db90d0647043f8c60147fc9045250bf
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351221"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/x509Certificate"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAuthenticationMethodConfiguration *authenticationMethodConfiguration = [[MSGraphAuthenticationMethodConfiguration alloc] init];
[authenticationMethodConfiguration setId:@"X509Certificate"];
[authenticationMethodConfiguration setState: [MSGraphAuthenticationMethodState enabled]];
NSMutableArray *certificateUserBindingsList = [[NSMutableArray alloc] init];
MSGraphX509CertificateUserBinding *certificateUserBindings = [[MSGraphX509CertificateUserBinding alloc] init];
[certificateUserBindings setX509CertificateField:@"PrincipalName"];
[certificateUserBindings setUserProperty:@"onPremisesUserPrincipalName"];
[certificateUserBindings setPriority: 1];
[certificateUserBindingsList addObject: certificateUserBindings];
[authenticationMethodConfiguration setCertificateUserBindings:certificateUserBindingsList];
MSGraphX509CertificateAuthenticationModeConfiguration *authenticationModeConfiguration = [[MSGraphX509CertificateAuthenticationModeConfiguration alloc] init];
[authenticationModeConfiguration setX509CertificateAuthenticationDefaultMode: [MSGraphX509CertificateAuthenticationMode x509CertificateMultiFactor]];
NSMutableArray *rulesList = [[NSMutableArray alloc] init];
MSGraphX509CertificateRule *rules = [[MSGraphX509CertificateRule alloc] init];
[rules setX509CertificateRuleType: [MSGraphX509CertificateRuleType issuerSubject]];
[rules setIdentifier:@"CN=ContosoCA,DC=Contoso,DC=org "];
[rules setX509CertificateAuthenticationMode: [MSGraphX509CertificateAuthenticationMode x509CertificateMultiFactor]];
[rulesList addObject: rules];
MSGraphX509CertificateRule *rules = [[MSGraphX509CertificateRule alloc] init];
[rules setX509CertificateRuleType: [MSGraphX509CertificateRuleType policyOID]];
[rules setIdentifier:@"1.2.3.4"];
[rules setX509CertificateAuthenticationMode: [MSGraphX509CertificateAuthenticationMode x509CertificateMultiFactor]];
[rulesList addObject: rules];
[authenticationModeConfiguration setRules:rulesList];
[authenticationMethodConfiguration setAuthenticationModeConfiguration:authenticationModeConfiguration];
NSMutableArray *includeTargetsList = [[NSMutableArray alloc] init];
MSGraphAuthenticationMethodTarget *includeTargets = [[MSGraphAuthenticationMethodTarget alloc] init];
[includeTargets setTargetType: [MSGraphAuthenticationMethodTargetType group]];
[includeTargets setId:@"all_users"];
[includeTargets setIsRegistrationRequired: false];
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