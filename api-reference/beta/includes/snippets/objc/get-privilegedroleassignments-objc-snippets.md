---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 051e2c10daba4c1d942dd158fb47ff17c067002a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720220"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *privilegedRoleAssignmentList = [[NSMutableArray alloc] init];
        privilegedRoleAssignmentList = [jsonFinal valueForKey:@"value"];
        MSGraphPrivilegedRoleAssignment *privilegedRoleAssignment = [[MSGraphPrivilegedRoleAssignment alloc] initWithDictionary:[privilegedRoleAssignmentList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```