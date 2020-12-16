---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 427d672229a1e7e8b6075c07186170fc9feb8cb8
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691415"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/authorizationPolicy"]]];
[urlRequest setHTTPMethod:@"PATCH"];

MSGraphAuthorizationPolicy *authorizationPolicy = [[MSGraphAuthorizationPolicy alloc] init];
MSGraphDefaultUserRolePermissions *defaultUserRolePermissions = [[MSGraphDefaultUserRolePermissions alloc] init];
NSMutableArray *permissionGrantPoliciesAssignedList = [[NSMutableArray alloc] init];
[defaultUserRolePermissions setPermissionGrantPoliciesAssigned:permissionGrantPoliciesAssignedList];
[authorizationPolicy setDefaultUserRolePermissions:defaultUserRolePermissions];

NSError *error;
NSData *authorizationPolicyData = [authorizationPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:authorizationPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```