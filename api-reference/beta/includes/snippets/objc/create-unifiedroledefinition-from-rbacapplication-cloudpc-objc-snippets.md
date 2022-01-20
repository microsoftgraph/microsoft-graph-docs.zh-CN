---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92c09578140cc6172415eb2cb16ce201b234c18b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120034"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/cloudPc/roleDefinitions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUnifiedRoleDefinition *unifiedRoleDefinition = [[MSGraphUnifiedRoleDefinition alloc] init];
[unifiedRoleDefinition setDescription:@"An example custom role"];
[unifiedRoleDefinition setDisplayName:@"ExampleCustomRole"];
NSMutableArray *rolePermissionsList = [[NSMutableArray alloc] init];
MSGraphUnifiedRolePermission *rolePermissions = [[MSGraphUnifiedRolePermission alloc] init];
NSMutableArray *allowedResourceActionsList = [[NSMutableArray alloc] init];
[allowedResourceActionsList addObject: @"Microsoft.CloudPC/CloudPCs/Read"];
[rolePermissions setAllowedResourceActions:allowedResourceActionsList];
[rolePermissionsList addObject: rolePermissions];
[unifiedRoleDefinition setRolePermissions:rolePermissionsList];
[unifiedRoleDefinition setCondition:@"null"];

NSError *error;
NSData *unifiedRoleDefinitionData = [unifiedRoleDefinition getSerializedDataWithError:&error];
[urlRequest setHTTPBody:unifiedRoleDefinitionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```