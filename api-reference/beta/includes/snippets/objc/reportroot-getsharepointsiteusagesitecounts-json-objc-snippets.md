---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 64cc8c5a10be220620d545f2e2066cd6cd02b88c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499615"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSharePointSiteUsageSiteCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *sharePointSiteUsageSiteCountsList = [[NSMutableArray alloc] init];
        sharePointSiteUsageSiteCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSharePointSiteUsageSiteCounts *sharePointSiteUsageSiteCounts = [[MSGraphSharePointSiteUsageSiteCounts alloc] initWithDictionary:[sharePointSiteUsageSiteCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```