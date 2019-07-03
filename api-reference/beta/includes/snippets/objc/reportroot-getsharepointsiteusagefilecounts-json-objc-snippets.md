---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 783b11afecb1f4f65f7e78b785c98767a723b853
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499850"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSharePointSiteUsageFileCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *sharePointSiteUsageFileCountsList = [[NSMutableArray alloc] init];
        sharePointSiteUsageFileCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSharePointSiteUsageFileCounts *sharePointSiteUsageFileCounts = [[MSGraphSharePointSiteUsageFileCounts alloc] initWithDictionary:[sharePointSiteUsageFileCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```