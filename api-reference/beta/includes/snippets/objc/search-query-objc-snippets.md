---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f1a1728ea822a9495569717873633583a210e66
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48230711"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/search/query"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *requestsList = [[NSMutableArray alloc] init];
MSGraphSearchRequest *requests = [[MSGraphSearchRequest alloc] init];
NSMutableArray *entityTypesList = [[NSMutableArray alloc] init];
[entityTypesList addObject: @"externalItem"];
[requests setEntityTypes:entityTypesList];
NSMutableArray *contentSourcesList = [[NSMutableArray alloc] init];
[contentSourcesList addObject: @"/external/connections/connectionfriendlyname"];
[requests setContentSources:contentSourcesList];
MSGraphSearchQuery *query = [[MSGraphSearchQuery alloc] init];
[query setQueryString:@"contoso product"];
[requests setQuery:query];
[requests setFrom: 0];
[requests setSize: 25];
NSMutableArray *fieldsList = [[NSMutableArray alloc] init];
[fieldsList addObject: @"title"];
[fieldsList addObject: @"description"];
[requests setFields:fieldsList];
[requestsList addObject: requests];
payloadDictionary[@"requests"] = requestsList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```