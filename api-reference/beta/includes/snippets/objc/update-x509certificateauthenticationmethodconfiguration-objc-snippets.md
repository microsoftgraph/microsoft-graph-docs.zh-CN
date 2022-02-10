---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26a70c78b5d65a28cfab0ae2db3b009e9bce2d0a
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519379"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/x509Certificate"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAuthenticationMethodConfiguration *authenticationMethodConfiguration = [[MSGraphAuthenticationMethodConfiguration alloc] init];
[authenticationMethodConfiguration setId:@"X509Certificate"];
[authenticationMethodConfiguration setState: [MSGraphAuthenticationMethodState disabled]];
NSMutableArray *certificateUserBindingsList = [[NSMutableArray alloc] init];
MSGraphX509CertificateUserBinding *certificateUserBindings = [[MSGraphX509CertificateUserBinding alloc] init];
[certificateUserBindings setX509CertificateField:@"PrincipalName"];
[certificateUserBindings setUserProperty:@"onPremisesUserPrincipalName"];
[certificateUserBindings setPriority: 1];
[certificateUserBindingsList addObject: certificateUserBindings];
MSGraphX509CertificateUserBinding *certificateUserBindings = [[MSGraphX509CertificateUserBinding alloc] init];
[certificateUserBindings setX509CertificateField:@"RFC822Name"];
[certificateUserBindings setUserProperty:@"userPrincipalName"];
[certificateUserBindings setPriority: 2];
[certificateUserBindingsList addObject: certificateUserBindings];
[authenticationMethodConfiguration setCertificateUserBindings:certificateUserBindingsList];
MSGraphX509CertificateAuthenticationModeConfiguration *authenticationModeConfiguration = [[MSGraphX509CertificateAuthenticationModeConfiguration alloc] init];
[authenticationModeConfiguration setX509CertificateAuthenticationDefaultMode: [MSGraphX509CertificateAuthenticationMode x509CertificateSingleFactor]];
NSMutableArray *rulesList = [[NSMutableArray alloc] init];
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