---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e58894366c4f6e82176c6aa4375b039dc27fad5dc74a7ef96116d8ae58bc9f39
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279728"
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