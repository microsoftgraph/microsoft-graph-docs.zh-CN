---
description: 自动生成的文件。 不修改
ms.openlocfilehash: eeed26a2f8297241814336237d2c6819beb5599f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330417"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *yammerDeviceUsageDistributionUserCountsList = [[NSMutableArray alloc] init];
        yammerDeviceUsageDistributionUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphYammerDeviceUsageDistributionUserCounts *yammerDeviceUsageDistributionUserCounts = [[MSGraphYammerDeviceUsageDistributionUserCounts alloc] initWithDictionary:[yammerDeviceUsageDistributionUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```