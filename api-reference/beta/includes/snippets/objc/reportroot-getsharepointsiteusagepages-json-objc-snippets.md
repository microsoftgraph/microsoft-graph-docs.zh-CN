---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f265057a7356e9085169aa350493020ca7ad387a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499847"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSharePointSiteUsagePages(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *sharePointSiteUsagePagesList = [[NSMutableArray alloc] init];
        sharePointSiteUsagePagesList = [jsonFinal valueForKey:@"value"];
        MSGraphSharePointSiteUsagePages *sharePointSiteUsagePages = [[MSGraphSharePointSiteUsagePages alloc] initWithDictionary:[sharePointSiteUsagePagesList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```