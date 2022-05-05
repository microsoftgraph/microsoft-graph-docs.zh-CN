---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c758c4594539544008561ef789e3d9355c65072a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206983"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/entitlementManagement/roleAssignments"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUnifiedRoleAssignment *unifiedRoleAssignment = [[MSGraphUnifiedRoleAssignment alloc] init];
[unifiedRoleAssignment setPrincipalId:@"679a9213-c497-48a4-830a-8d3d25d94ddc"];
[unifiedRoleAssignment setRoleDefinitionId:@"ae79f266-94d4-4dab-b730-feca7e132178"];
[unifiedRoleAssignment setAppScopeId:@"/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997"];

NSError *error;
NSData *unifiedRoleAssignmentData = [unifiedRoleAssignment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:unifiedRoleAssignmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```