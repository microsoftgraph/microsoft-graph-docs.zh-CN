---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d160701a375e268caaa2aab6de9e23d29e3fea97
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858757"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/delta?$select=displayName,description,mailNickname"]]];
[urlRequest setHTTPMethod:@"GET"];
[urlRequest setValue:@"return=minimal" forHTTPHeaderField:@"Prefer"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *groupList = [[NSMutableArray alloc] init];
        groupList = [jsonFinal valueForKey:@"value"];
        MSGraphGroup *group = [[MSGraphGroup alloc] initWithDictionary:[groupList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```