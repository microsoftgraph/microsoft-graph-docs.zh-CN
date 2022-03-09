---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b400ba2cf5857bb2cb5f2aed4843b55c3f383a21
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394696"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/defaultAppManagementPolicy"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTenantAppManagementPolicy *tenantAppManagementPolicy = [[MSGraphTenantAppManagementPolicy alloc] init];
[tenantAppManagementPolicy setIsEnabled: true];
MSGraphAppManagementConfiguration *applicationRestrictions = [[MSGraphAppManagementConfiguration alloc] init];
NSMutableArray *passwordCredentialsList = [[NSMutableArray alloc] init];
MSGraphPasswordCredentialConfiguration *passwordCredentials = [[MSGraphPasswordCredentialConfiguration alloc] init];
[passwordCredentials setRestrictionType: [MSGraphAppCredentialRestrictionType passwordAddition]];
[passwordCredentials setMaxLifetime: null];
[passwordCredentials setRestrictForAppsCreatedAfterDateTime: "2021-01-01T10:37:00Z"];
[passwordCredentialsList addObject: passwordCredentials];
MSGraphPasswordCredentialConfiguration *passwordCredentials = [[MSGraphPasswordCredentialConfiguration alloc] init];
[passwordCredentials setRestrictionType: [MSGraphAppCredentialRestrictionType passwordLifetime]];
[passwordCredentials setMaxLifetime:@"P4DT12H30M5S"];
[passwordCredentials setRestrictForAppsCreatedAfterDateTime: "2017-01-01T10:37:00Z"];
[passwordCredentialsList addObject: passwordCredentials];
MSGraphPasswordCredentialConfiguration *passwordCredentials = [[MSGraphPasswordCredentialConfiguration alloc] init];
[passwordCredentials setRestrictionType: [MSGraphAppCredentialRestrictionType symmetricKeyAddition]];
[passwordCredentials setMaxLifetime: null];
[passwordCredentials setRestrictForAppsCreatedAfterDateTime: "2021-01-01T10:37:00Z"];
[passwordCredentialsList addObject: passwordCredentials];
MSGraphPasswordCredentialConfiguration *passwordCredentials = [[MSGraphPasswordCredentialConfiguration alloc] init];
[passwordCredentials setRestrictionType: [MSGraphAppCredentialRestrictionType customPasswordAddition]];
[passwordCredentials setMaxLifetime: null];
[passwordCredentials setRestrictForAppsCreatedAfterDateTime: "2015-01-01T10:37:00Z"];
[passwordCredentialsList addObject: passwordCredentials];
MSGraphPasswordCredentialConfiguration *passwordCredentials = [[MSGraphPasswordCredentialConfiguration alloc] init];
[passwordCredentials setRestrictionType: [MSGraphAppCredentialRestrictionType symmetricKeyLifetime]];
[passwordCredentials setMaxLifetime:@"P40D"];
[passwordCredentials setRestrictForAppsCreatedAfterDateTime: "2015-01-01T10:37:00Z"];
[passwordCredentialsList addObject: passwordCredentials];
[applicationRestrictions setPasswordCredentials:passwordCredentialsList];
NSMutableArray *keyCredentialsList = [[NSMutableArray alloc] init];
MSGraphKeyCredentialConfiguration *keyCredentials = [[MSGraphKeyCredentialConfiguration alloc] init];
[keyCredentials setRestrictionType: [MSGraphAppKeyCredentialRestrictionType asymmetricKeyLifetime]];
[keyCredentials setMaxLifetime:@"P30D"];
[keyCredentials setRestrictForAppsCreatedAfterDateTime: "2015-01-01T10:37:00Z"];
[keyCredentialsList addObject: keyCredentials];
[applicationRestrictions setKeyCredentials:keyCredentialsList];
[tenantAppManagementPolicy setApplicationRestrictions:applicationRestrictions];

NSError *error;
NSData *tenantAppManagementPolicyData = [tenantAppManagementPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:tenantAppManagementPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```