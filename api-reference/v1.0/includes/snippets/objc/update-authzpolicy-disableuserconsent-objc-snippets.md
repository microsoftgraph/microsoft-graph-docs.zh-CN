---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89290b6ef9053854f868abc5a339ca8c43de02a13a9d3e2d8ab19f9efbfb701d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332200"
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