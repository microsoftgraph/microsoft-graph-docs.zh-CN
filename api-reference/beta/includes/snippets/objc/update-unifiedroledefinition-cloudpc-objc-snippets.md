---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a247e71a998f02dccbe13fc86fc4942662dc410
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089127"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/cloudPc/roleDefinitions/b7f5ddc1-b7dc-4d37-abce-b9d6fc15ffff"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUnifiedRoleDefinition *unifiedRoleDefinition = [[MSGraphUnifiedRoleDefinition alloc] init];
[unifiedRoleDefinition setDescription:@"Update basic properties and permission of application registrations"];
[unifiedRoleDefinition setDisplayName:@"ExampleCustomRole"];
NSMutableArray *rolePermissionsList = [[NSMutableArray alloc] init];
MSGraphUnifiedRolePermission *rolePermissions = [[MSGraphUnifiedRolePermission alloc] init];
NSMutableArray *allowedResourceActionsList = [[NSMutableArray alloc] init];
[allowedResourceActionsList addObject: @"Microsoft.CloudPC/CloudPCs/Read"];
[allowedResourceActionsList addObject: @"Microsoft.CloudPC/CloudPCs/Reprovision"];
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