---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 748cb549032f9a0a16ef01331fcecc01e2cf65c8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210801"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/delegatedAdminRelationships/72a7ae7e-4887-4e34-9755-2e1e9b26b943-63f017cb-9e0d-4f14-94bd-4871902b3409/accessAssignments"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDelegatedAdminAccessAssignment *delegatedAdminAccessAssignment = [[MSGraphDelegatedAdminAccessAssignment alloc] init];
MSGraphDelegatedAdminAccessContainer *accessContainer = [[MSGraphDelegatedAdminAccessContainer alloc] init];
[accessContainer setAccessContainerId:@"869713c9-0b28-4d08-8949-ae07ae1bf528"];
[accessContainer setAccessContainerType: [MSGraphDelegatedAdminAccessContainerType securityGroup]];
[delegatedAdminAccessAssignment setAccessContainer:accessContainer];
MSGraphDelegatedAdminAccessDetails *accessDetails = [[MSGraphDelegatedAdminAccessDetails alloc] init];
NSMutableArray *unifiedRolesList = [[NSMutableArray alloc] init];
MSGraphUnifiedRole *unifiedRoles = [[MSGraphUnifiedRole alloc] init];
[unifiedRoles setRoleDefinitionId:@"29232cdf-9323-42fd-ade2-1d097af3e4de"];
[unifiedRolesList addObject: unifiedRoles];
MSGraphUnifiedRole *unifiedRoles = [[MSGraphUnifiedRole alloc] init];
[unifiedRoles setRoleDefinitionId:@"f2ef992c-3afb-46b9-b7cf-a126ee74c451"];
[unifiedRolesList addObject: unifiedRoles];
MSGraphUnifiedRole *unifiedRoles = [[MSGraphUnifiedRole alloc] init];
[unifiedRoles setRoleDefinitionId:@"729827e3-9c14-49f7-bb1b-9608f156bbb8"];
[unifiedRolesList addObject: unifiedRoles];
MSGraphUnifiedRole *unifiedRoles = [[MSGraphUnifiedRole alloc] init];
[unifiedRoles setRoleDefinitionId:@"3a2c62db-5318-420d-8d74-23affee5d9d5"];
[unifiedRolesList addObject: unifiedRoles];
[accessDetails setUnifiedRoles:unifiedRolesList];
[delegatedAdminAccessAssignment setAccessDetails:accessDetails];

NSError *error;
NSData *delegatedAdminAccessAssignmentData = [delegatedAdminAccessAssignment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:delegatedAdminAccessAssignmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```