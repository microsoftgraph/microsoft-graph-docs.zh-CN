---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bb89f151998d65ba8fba233b7f842cb515b10b11df7a2f88d5ddc359cf30a4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54275340"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/deviceManagement/roleAssignments"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUnifiedRoleAssignmentMultiple *unifiedRoleAssignmentMultiple = [[MSGraphUnifiedRoleAssignmentMultiple alloc] init];
[unifiedRoleAssignmentMultiple setDisplayName:@"My test role assignment 1"];
[unifiedRoleAssignmentMultiple setRoleDefinitionId:@"c2cf284d-6c41-4e6b-afac-4b80928c9034"];
NSMutableArray *principalIdsList = [[NSMutableArray alloc] init];
[principalIdsList addObject: @"f8ca5a85-489a-49a0-b555-0a6d81e56f0d"];
[principalIdsList addObject: @"c1518aa9-4da5-4c84-a902-a31404023890"];
[unifiedRoleAssignmentMultiple setPrincipalIds:principalIdsList];
NSMutableArray *directoryScopeIdsList = [[NSMutableArray alloc] init];
[directoryScopeIdsList addObject: @"28ca5a85-489a-49a0-b555-0a6d81e56f0d"];
[directoryScopeIdsList addObject: @"8152656a-cf9a-4928-a457-1512d4cae295"];
[unifiedRoleAssignmentMultiple setDirectoryScopeIds:directoryScopeIdsList];

NSError *error;
NSData *unifiedRoleAssignmentMultipleData = [unifiedRoleAssignmentMultiple getSerializedDataWithError:&error];
[urlRequest setHTTPBody:unifiedRoleAssignmentMultipleData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```