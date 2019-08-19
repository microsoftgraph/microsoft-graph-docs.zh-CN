---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3ce177e87823291e4d12c795316db39fd7828844
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461608"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleDefinitions/0d55728d-3e24-4309-9b1b-5ac09921475a"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUnifiedRoleDefinition *unifiedRoleDefinition = [[MSGraphUnifiedRoleDefinition alloc] init];
[unifiedRoleDefinition setDescription:@"Update basic properties of application registrations"];
[unifiedRoleDefinition setDisplayName:@"Application Registration Support Administrator"];
NSMutableArray *rolePermissionsList = [[NSMutableArray alloc] init];
MSGraphUnifiedRolePermission *rolePermissions = [[MSGraphUnifiedRolePermission alloc] init];
NSMutableArray *allowedResourceActionsList = [[NSMutableArray alloc] init];
[allowedResourceActionsList addObject: @"microsoft.directory/applications/basic/read"];
[rolePermissions setAllowedResourceActions:allowedResourceActionsList];
[rolePermissionsList addObject: rolePermissions];
[unifiedRoleDefinition setRolePermissions:rolePermissionsList];

NSError *error;
NSData *unifiedRoleDefinitionData = [unifiedRoleDefinition getSerializedDataWithError:&error];
[urlRequest setHTTPBody:unifiedRoleDefinitionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```