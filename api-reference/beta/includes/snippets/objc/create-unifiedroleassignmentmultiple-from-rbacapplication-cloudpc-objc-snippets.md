---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f4de3498c3449a8e5be2c72a086df71923fb151
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868965"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/cloudPC/roleAssignments"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUnifiedRoleAssignmentMultiple *unifiedRoleAssignmentMultiple = [[MSGraphUnifiedRoleAssignmentMultiple alloc] init];
[unifiedRoleAssignmentMultiple setDisplayName:@"My test role assignment 1"];
[unifiedRoleAssignmentMultiple setDescription:@"My role assignment description"];
[unifiedRoleAssignmentMultiple setRoleDefinitionId:@"b5c08161-a7af-481c-ace2-a20a69a48fb1"];
NSMutableArray *principalIdsList = [[NSMutableArray alloc] init];
[principalIdsList addObject: @"f8ca5a85-489a-49a0-b555-0a6d81e56f0d"];
[principalIdsList addObject: @"c1518aa9-4da5-4c84-a902-a31404023890"];
[unifiedRoleAssignmentMultiple setPrincipalIds:principalIdsList];

NSError *error;
NSData *unifiedRoleAssignmentMultipleData = [unifiedRoleAssignmentMultiple getSerializedDataWithError:&error];
[urlRequest setHTTPBody:unifiedRoleAssignmentMultipleData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```