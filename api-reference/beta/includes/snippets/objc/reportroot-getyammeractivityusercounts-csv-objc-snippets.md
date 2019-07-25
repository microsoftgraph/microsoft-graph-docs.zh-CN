---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c082ed8a3a5b70cd46e01d80a02d9b9e460e6a26
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726421"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getYammerActivityUserCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *yammerActivitySummaryList = [[NSMutableArray alloc] init];
        yammerActivitySummaryList = [jsonFinal valueForKey:@"value"];
        MSGraphYammerActivitySummary *yammerActivitySummary = [[MSGraphYammerActivitySummary alloc] initWithDictionary:[yammerActivitySummaryList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```