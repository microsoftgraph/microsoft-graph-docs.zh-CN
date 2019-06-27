---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8460b2a2c6b0b845d002729766eb9a6ae42cabf7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330098"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getYammerGroupsActivityGroupCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *yammerGroupsActivityGroupCountsList = [[NSMutableArray alloc] init];
        yammerGroupsActivityGroupCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphYammerGroupsActivityGroupCounts *yammerGroupsActivityGroupCounts = [[MSGraphYammerGroupsActivityGroupCounts alloc] initWithDictionary:[yammerGroupsActivityGroupCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```