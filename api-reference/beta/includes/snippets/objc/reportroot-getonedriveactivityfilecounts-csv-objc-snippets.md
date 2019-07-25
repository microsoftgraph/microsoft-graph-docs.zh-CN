---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e576610ee81f36d6552565bdae642a6cc5b5d362
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727215"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOneDriveActivityFileCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *siteActivitySummaryList = [[NSMutableArray alloc] init];
        siteActivitySummaryList = [jsonFinal valueForKey:@"value"];
        MSGraphSiteActivitySummary *siteActivitySummary = [[MSGraphSiteActivitySummary alloc] initWithDictionary:[siteActivitySummaryList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```