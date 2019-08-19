---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ac9a573e5e44b128ee12b26f3d36628f12bc2e19
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461398"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleAssignments?$filter=principalId%20eq%20'a98eb769-7bd4-4489-86f6-ad96e1d58b62'"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *unifiedRoleAssignmentList = [[NSMutableArray alloc] init];
        unifiedRoleAssignmentList = [jsonFinal valueForKey:@"value"];
        MSGraphUnifiedRoleAssignment *unifiedRoleAssignment = [[MSGraphUnifiedRoleAssignment alloc] initWithDictionary:[unifiedRoleAssignmentList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```