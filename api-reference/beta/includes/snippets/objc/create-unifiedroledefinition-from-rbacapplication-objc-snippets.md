---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef449b27d0b6aac6aa80c36c2eca2fd243aabbd22d8d0eb8a693b204761fbc38
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279032"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleDefinitions"]]];
[urlRequest setHTTPMethod:@"POST"];
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
[unifiedRoleDefinition setIsEnabled:@"true"];

NSError *error;
NSData *unifiedRoleDefinitionData = [unifiedRoleDefinition getSerializedDataWithError:&error];
[urlRequest setHTTPBody:unifiedRoleDefinitionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```