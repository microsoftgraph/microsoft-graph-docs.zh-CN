---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 978752b38a56763847c160d9fdfb2d3c54bcd6af
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719596"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getEmailAppUsageAppsUserCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *emailAppUsageAppsUserCountsList = [[NSMutableArray alloc] init];
        emailAppUsageAppsUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphEmailAppUsageAppsUserCounts *emailAppUsageAppsUserCounts = [[MSGraphEmailAppUsageAppsUserCounts alloc] initWithDictionary:[emailAppUsageAppsUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```