---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7a8a92015e9d3d997d02a7c75c83a83ed2913757
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718486"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *teamsUserActivityUserCountsList = [[NSMutableArray alloc] init];
        teamsUserActivityUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphTeamsUserActivityUserCounts *teamsUserActivityUserCounts = [[MSGraphTeamsUserActivityUserCounts alloc] initWithDictionary:[teamsUserActivityUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```