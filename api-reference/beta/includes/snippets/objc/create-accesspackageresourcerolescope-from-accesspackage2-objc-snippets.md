---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0606db52d81a8d95171a1d29c8102fe62031f101
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439876"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessPackageResourceRoleScope *accessPackageResourceRoleScope = [[MSGraphAccessPackageResourceRoleScope alloc] init];
MSGraphAccessPackageResourceRole *accessPackageResourceRole = [[MSGraphAccessPackageResourceRole alloc] init];
[accessPackageResourceRole setOriginId:@"4"];
[accessPackageResourceRole setOriginSystem:@"SharePointOnline"];
MSGraphAccessPackageResource *accessPackageResource = [[MSGraphAccessPackageResource alloc] init];
[accessPackageResource setId:@"53c71803-a0a8-4777-aecc-075de8ee3991"];
[accessPackageResourceRole setAccessPackageResource:accessPackageResource];
[accessPackageResourceRoleScope setAccessPackageResourceRole:accessPackageResourceRole];
MSGraphAccessPackageResourceScope *accessPackageResourceScope = [[MSGraphAccessPackageResourceScope alloc] init];
[accessPackageResourceScope setId:@"5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33"];
[accessPackageResourceScope setOriginId:@"https://microsoft.sharepoint.com/portals/Community"];
[accessPackageResourceScope setOriginSystem:@"SharePointOnline"];
[accessPackageResourceRoleScope setAccessPackageResourceScope:accessPackageResourceScope];

NSError *error;
NSData *accessPackageResourceRoleScopeData = [accessPackageResourceRoleScope getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessPackageResourceRoleScopeData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```