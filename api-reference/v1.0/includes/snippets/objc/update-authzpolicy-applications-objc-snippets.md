---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15d4ea29b2221cbd756b4f19c5d8ba4f5eacadd4
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691418"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/authorizationPolicy"]]];
[urlRequest setHTTPMethod:@"PATCH"];

MSGraphAuthorizationPolicy *authorizationPolicy = [[MSGraphAuthorizationPolicy alloc] init];
MSGraphDefaultUserRolePermissions *defaultUserRolePermissions = [[MSGraphDefaultUserRolePermissions alloc] init];
[defaultUserRolePermissions setAllowedToCreateApps: false];
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