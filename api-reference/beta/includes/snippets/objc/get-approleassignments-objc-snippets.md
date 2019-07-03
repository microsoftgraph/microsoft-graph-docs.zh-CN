---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 259a86a0a8f6f89a9f2f3dee0dc02efc01fbc8d3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479891"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/appRoleAssignments"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *appRoleAssignmentList = [[NSMutableArray alloc] init];
        appRoleAssignmentList = [jsonFinal valueForKey:@"value"];
        MSGraphAppRoleAssignment *appRoleAssignment = [[MSGraphAppRoleAssignment alloc] initWithDictionary:[appRoleAssignmentList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```