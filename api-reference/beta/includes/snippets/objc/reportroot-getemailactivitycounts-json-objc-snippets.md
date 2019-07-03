---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 14f6cc0405a72a803f69e8452e7cb190c9f75629
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500071"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getEmailActivityCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *emailActivitySummaryList = [[NSMutableArray alloc] init];
        emailActivitySummaryList = [jsonFinal valueForKey:@"value"];
        MSGraphEmailActivitySummary *emailActivitySummary = [[MSGraphEmailActivitySummary alloc] initWithDictionary:[emailActivitySummaryList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```