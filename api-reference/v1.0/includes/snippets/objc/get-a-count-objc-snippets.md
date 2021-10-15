---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 979ecbda35883f3363796335b6327e6b8b4403cc
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2021
ms.locfileid: "59766229"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/contacts?$filter=startswith(displayName,'A')&$count=true&$top=1&$orderby=displayName"]]];
[urlRequest setHTTPMethod:@"GET"];
[urlRequest setValue:@"eventual" forHTTPHeaderField:@"ConsistencyLevel"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphOrgContact *orgContact = [[MSGraphOrgContact alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```