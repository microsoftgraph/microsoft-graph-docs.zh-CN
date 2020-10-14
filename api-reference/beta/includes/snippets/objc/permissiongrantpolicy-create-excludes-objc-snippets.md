---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7383749e37594958817f8715af83c519345201a6
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458696"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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