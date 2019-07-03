---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bcc32fbcfc91e5499ade8e75fb9ca5d7e4533e57
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478148"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSharePointActivityUserCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *sharePointActivityUserCountsList = [[NSMutableArray alloc] init];
        sharePointActivityUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSharePointActivityUserCounts *sharePointActivityUserCounts = [[MSGraphSharePointActivityUserCounts alloc] initWithDictionary:[sharePointActivityUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```