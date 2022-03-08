---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ff72c1d9ccbecaf4a0475b10df0fce9e2663b3b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336639"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/crossTenantAccessPolicy"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCrossTenantAccessPolicy *crossTenantAccessPolicy = [[MSGraphCrossTenantAccessPolicy alloc] init];
[crossTenantAccessPolicy setDisplayName:@"CrossTenantAccessPolicy"];

NSError *error;
NSData *crossTenantAccessPolicyData = [crossTenantAccessPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:crossTenantAccessPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```