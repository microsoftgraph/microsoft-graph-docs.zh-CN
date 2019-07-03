---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1d6ac6e15e6bbed2b0ee9ea4cd8d5d4264a697c6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520441"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getEmailAppUsageUserCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *emailAppUsageUserCountsList = [[NSMutableArray alloc] init];
        emailAppUsageUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphEmailAppUsageUserCounts *emailAppUsageUserCounts = [[MSGraphEmailAppUsageUserCounts alloc] initWithDictionary:[emailAppUsageUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```