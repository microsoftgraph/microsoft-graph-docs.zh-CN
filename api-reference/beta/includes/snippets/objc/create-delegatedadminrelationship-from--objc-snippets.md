---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0af3dcfe458e4ea0082a2ca53ddc50e21ffd05e0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205434"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/delegatedAdminRelationships"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDelegatedAdminRelationship *delegatedAdminRelationship = [[MSGraphDelegatedAdminRelationship alloc] init];
[delegatedAdminRelationship setDisplayName:@"Contoso admin relationship"];
[delegatedAdminRelationship setDuration:@"P730D"];
MSGraphDelegatedAdminRelationshipCustomerParticipant *customer = [[MSGraphDelegatedAdminRelationshipCustomerParticipant alloc] init];
[customer setTenantId:@"4b827261-d21f-4aa9-b7db-7fa1f56fb163"];
[customer setDisplayName:@"Contoso subsidiary Inc"];
[delegatedAdminRelationship setCustomer:customer];
MSGraphDelegatedAdminAccessDetails *accessDetails = [[MSGraphDelegatedAdminAccessDetails alloc] init];
NSMutableArray *unifiedRolesList = [[NSMutableArray alloc] init];
MSGraphUnifiedRole *unifiedRoles = [[MSGraphUnifiedRole alloc] init];
[unifiedRoles setRoleDefinitionId:@"29232cdf-9323-42fd-ade2-1d097af3e4de"];
[unifiedRolesList addObject: unifiedRoles];
MSGraphUnifiedRole *unifiedRoles = [[MSGraphUnifiedRole alloc] init];
[unifiedRoles setRoleDefinitionId:@"3a2c62db-5318-420d-8d74-23affee5d9d5"];
[unifiedRolesList addObject: unifiedRoles];
[accessDetails setUnifiedRoles:unifiedRolesList];
[delegatedAdminRelationship setAccessDetails:accessDetails];

NSError *error;
NSData *delegatedAdminRelationshipData = [delegatedAdminRelationship getSerializedDataWithError:&error];
[urlRequest setHTTPBody:delegatedAdminRelationshipData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```