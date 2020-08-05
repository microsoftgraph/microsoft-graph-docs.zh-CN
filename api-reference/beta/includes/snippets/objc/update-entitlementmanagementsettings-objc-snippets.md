---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9b7b41941459cd405b31c93904671a2ae9b5018
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566860"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/settings"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEntitlementManagementSettings *entitlementManagementSettings = [[MSGraphEntitlementManagementSettings alloc] init];
[entitlementManagementSettings setExternalUserLifecycleAction:@"None"];

NSError *error;
NSData *entitlementManagementSettingsData = [entitlementManagementSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:entitlementManagementSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```