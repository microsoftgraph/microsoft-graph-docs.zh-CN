---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd79785971a6d535c104e43fe928c2b6246c27b8ea7fc30ad8fa89eedc267904
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220512"
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