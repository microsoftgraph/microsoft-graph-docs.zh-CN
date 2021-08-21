---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cdfa8e9a047f3a65ec5ae1b3aac23b79a3c4832bcabf7871630c04b254249d84
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219115"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedRoleAssignments?$filter=isElevated%20eq%20true"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphPrivilegedRoleAssignment *privilegedRoleAssignment = [[MSGraphPrivilegedRoleAssignment alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```