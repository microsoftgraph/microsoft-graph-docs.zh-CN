---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bf449e05a97b2f74ba5b4117d904bde575d04ae4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726547"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *teamsUserActivityCountsList = [[NSMutableArray alloc] init];
        teamsUserActivityCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphTeamsUserActivityCounts *teamsUserActivityCounts = [[MSGraphTeamsUserActivityCounts alloc] initWithDictionary:[teamsUserActivityCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```