---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b43dc77a9946096f0c18e174f7c3ba463975ed37
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35315645"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessDeviceUsageUserCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessDeviceUsageUserCountsList = [[NSMutableArray alloc] init];
        skypeForBusinessDeviceUsageUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessDeviceUsageUserCounts *skypeForBusinessDeviceUsageUserCounts = [[MSGraphSkypeForBusinessDeviceUsageUserCounts alloc] initWithDictionary:[skypeForBusinessDeviceUsageUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```