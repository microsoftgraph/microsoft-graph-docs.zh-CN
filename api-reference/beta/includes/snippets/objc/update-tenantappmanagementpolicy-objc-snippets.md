---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29ec480be59a445cad0094b10be0bdafcf035155
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696094"
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
[passwordCredentials setRestrictForAppsCreatedAfterDateTime: "2021-04-01T10:37:00Z"];
[passwordCredentialsList addObject: passwordCredentials];
MSGraphPasswordCredentialConfiguration *passwordCredentials = [[MSGraphPasswordCredentialConfiguration alloc] init];
[passwordCredentials setRestrictionType: [MSGraphAppCredentialRestrictionType passwordLifetime]];
[passwordCredentials setMaxLifetime:@"P4DT12H30M5S"];
[passwordCredentials setRestrictForAppsCreatedAfterDateTime: "2019-01-01T10:37:00Z"];
[passwordCredentialsList addObject: passwordCredentials];
MSGraphPasswordCredentialConfiguration *passwordCredentials = [[MSGraphPasswordCredentialConfiguration alloc] init];
[passwordCredentials setRestrictionType: [MSGraphAppCredentialRestrictionType symmetricKeyAddition]];
[passwordCredentials setMaxLifetime: null];
[passwordCredentials setRestrictForAppsCreatedAfterDateTime: "2021-04-01T10:37:00Z"];
[passwordCredentialsList addObject: passwordCredentials];
MSGraphPasswordCredentialConfiguration *passwordCredentials = [[MSGraphPasswordCredentialConfiguration alloc] init];
[passwordCredentials setRestrictionType: [MSGraphAppCredentialRestrictionType symmetricKeyLifetime]];
[passwordCredentials setMaxLifetime:@"P40D"];
[passwordCredentials setRestrictForAppsCreatedAfterDateTime: "2015-04-01T10:37:00Z"];
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