---
description: 自动生成的文件。 不修改
ms.openlocfilehash: efcac655dae7126be497be21db662a2afde3d15e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330060"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getEmailAppUsageVersionsUserCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *emailAppUsageVersionsUserCountsList = [[NSMutableArray alloc] init];
        emailAppUsageVersionsUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphEmailAppUsageVersionsUserCounts *emailAppUsageVersionsUserCounts = [[MSGraphEmailAppUsageVersionsUserCounts alloc] initWithDictionary:[emailAppUsageVersionsUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```