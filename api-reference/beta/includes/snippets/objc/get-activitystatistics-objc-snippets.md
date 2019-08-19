---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 38d8375ece35e10558bd73d8cb8e979c385c860d
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460782"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/analytics/activitystatistics"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *activityStatisticsList = [[NSMutableArray alloc] init];
        activityStatisticsList = [jsonFinal valueForKey:@"value"];
        MSGraphActivityStatistics *activityStatistics = [[MSGraphActivityStatistics alloc] initWithDictionary:[activityStatisticsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```