---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d66a8ba9150b19581d744525e12663d7aa67c64daaec3afd6fba31e174f84cc8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164288"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/permissionGrantPolicies/my-custom-consent-policy/excludes"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPermissionGrantConditionSet *permissionGrantConditionSet = [[MSGraphPermissionGrantConditionSet alloc] init];
[permissionGrantConditionSet setPermissionType: [MSGraphPermissionType delegated]];
[permissionGrantConditionSet setResourceApplication:@"00000003-0000-0000-c000-000000000000"];

NSError *error;
NSData *permissionGrantConditionSetData = [permissionGrantConditionSet getSerializedDataWithError:&error];
[urlRequest setHTTPBody:permissionGrantConditionSetData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```