---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 55aad94a8a7ccd83eb18821fa41d8b8d79cf2196
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330675"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getYammerGroupsActivityCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *yammerGroupsActivityCountsList = [[NSMutableArray alloc] init];
        yammerGroupsActivityCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphYammerGroupsActivityCounts *yammerGroupsActivityCounts = [[MSGraphYammerGroupsActivityCounts alloc] initWithDictionary:[yammerGroupsActivityCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```