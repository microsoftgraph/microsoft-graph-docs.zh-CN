---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc4dc30a7cd1fde5561208802ac0f2590ba805b2
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524133"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/permissionGrantPolicies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPermissionGrantPolicy *permissionGrantPolicy = [[MSGraphPermissionGrantPolicy alloc] init];
[permissionGrantPolicy setId:@"my-custom-consent-policy"];
[permissionGrantPolicy setDisplayName:@"Custom application consent policy"];
[permissionGrantPolicy setDescription:@"A custom permission grant policy to customize conditions for granting consent."];

NSError *error;
NSData *permissionGrantPolicyData = [permissionGrantPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:permissionGrantPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```