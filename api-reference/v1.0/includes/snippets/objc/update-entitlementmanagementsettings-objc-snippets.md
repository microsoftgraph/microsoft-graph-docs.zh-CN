---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e37b00f76d1d0b865a2f6f59fb8b8730c14debc
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336896"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/settings"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEntitlementManagementSettings *entitlementManagementSettings = [[MSGraphEntitlementManagementSettings alloc] init];
[entitlementManagementSettings setExternalUserLifecycleAction: [MSGraphAccessPackageExternalUserLifecycleAction none]];

NSError *error;
NSData *entitlementManagementSettingsData = [entitlementManagementSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:entitlementManagementSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```