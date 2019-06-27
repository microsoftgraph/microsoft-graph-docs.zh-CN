---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b4cb11c965d1367af8be29c14790cb549c2d1179
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35329960"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessOrganizerActivityMinuteCountsList = [[NSMutableArray alloc] init];
        skypeForBusinessOrganizerActivityMinuteCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessOrganizerActivityMinuteCounts *skypeForBusinessOrganizerActivityMinuteCounts = [[MSGraphSkypeForBusinessOrganizerActivityMinuteCounts alloc] initWithDictionary:[skypeForBusinessOrganizerActivityMinuteCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```