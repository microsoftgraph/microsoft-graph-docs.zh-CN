---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6baeb15b510b2e490ce49cbe7d5ceeaa5d5f1a70
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478144"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSharePointSiteUsageDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *sharePointSiteUsageDetailList = [[NSMutableArray alloc] init];
        sharePointSiteUsageDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphSharePointSiteUsageDetail *sharePointSiteUsageDetail = [[MSGraphSharePointSiteUsageDetail alloc] initWithDictionary:[sharePointSiteUsageDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```