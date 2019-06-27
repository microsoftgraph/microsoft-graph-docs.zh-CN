---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ba91e98c470ec90504ee635ae43b36b8f7f4e0c7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35318125"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json"]]];
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