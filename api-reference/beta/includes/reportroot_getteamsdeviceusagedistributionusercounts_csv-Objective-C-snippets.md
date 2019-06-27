---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8c4d186f715ab6176ea3104a2d1f11f16f443823
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35329918"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *teamsDeviceUsageDistributionUserCountsList = [[NSMutableArray alloc] init];
        teamsDeviceUsageDistributionUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphTeamsDeviceUsageDistributionUserCounts *teamsDeviceUsageDistributionUserCounts = [[MSGraphTeamsDeviceUsageDistributionUserCounts alloc] initWithDictionary:[teamsDeviceUsageDistributionUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```