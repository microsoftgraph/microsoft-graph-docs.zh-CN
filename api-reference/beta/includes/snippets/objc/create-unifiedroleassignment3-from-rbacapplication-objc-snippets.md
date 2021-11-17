---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75600967242a2798ceee92c900326c9fcfa12518bd14038cc26b420d64202cf2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163216"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/entitlementManagement/roleAssignments"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUnifiedRoleAssignment *unifiedRoleAssignment = [[MSGraphUnifiedRoleAssignment alloc] init];
[unifiedRoleAssignment setPrincipalId:@"679a9213-c497-48a4-830a-8d3d25d94ddc"];
[unifiedRoleAssignment setRoleDefinitionId:@"ae79f266-94d4-4dab-b730-feca7e132178"];
[unifiedRoleAssignment setAppScopeId:@"/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997"];

NSError *error;
NSData *unifiedRoleAssignmentData = [unifiedRoleAssignment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:unifiedRoleAssignmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```