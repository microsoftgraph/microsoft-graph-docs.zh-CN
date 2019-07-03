---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dde0b6344cb923d59dec76f0e31707ce3b3216d0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521450"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *teamsUserActivityUserDetailList = [[NSMutableArray alloc] init];
        teamsUserActivityUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphTeamsUserActivityUserDetail *teamsUserActivityUserDetail = [[MSGraphTeamsUserActivityUserDetail alloc] initWithDictionary:[teamsUserActivityUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```