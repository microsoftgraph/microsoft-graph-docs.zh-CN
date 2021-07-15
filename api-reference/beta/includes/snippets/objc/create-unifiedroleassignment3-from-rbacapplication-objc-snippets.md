---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54d3bea7c200e7f2ffc33b3bb456a2f5ed77e378
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442189"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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