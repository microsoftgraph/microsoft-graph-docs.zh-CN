---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 239a89a6538d64106d0b296b984d3a6de3958c353740bd5d6d79728ed5c99461
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218894"
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