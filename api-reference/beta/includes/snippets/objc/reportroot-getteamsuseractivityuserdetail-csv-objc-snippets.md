---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 104d5c05c4b816c23abde6e3db65345e2d70e8ef
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520689"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv"]]];
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