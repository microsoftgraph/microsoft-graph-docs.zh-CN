---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 88c6c7624db1acf5a481611f2d0524ff7ac34213
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520685"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/appRoleAssignments/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAppRoleAssignment *appRoleAssignment = [[MSGraphAppRoleAssignment alloc] init];
[appRoleAssignment setCreationTimestamp: "2016-10-19T10:37:00Z"];
[appRoleAssignment setPrincipalDisplayName:@"principalDisplayName-value"];
[appRoleAssignment setPrincipalId:@"principalId-value"];
[appRoleAssignment setPrincipalType:@"principalType-value"];
[appRoleAssignment setResourceDisplayName:@"resourceDisplayName-value"];

NSError *error;
NSData *appRoleAssignmentData = [appRoleAssignment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:appRoleAssignmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```