---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 983ec48d0efa6c1587c9e6af6d75c3dde7b8770b80e2c556968c23fbf254a01d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104214"
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