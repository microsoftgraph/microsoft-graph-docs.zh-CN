---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1e199c9e6af3b12774a9f0641c84ddd965c62f9d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478692"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessActivityUserCountsList = [[NSMutableArray alloc] init];
        skypeForBusinessActivityUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessActivityUserCounts *skypeForBusinessActivityUserCounts = [[MSGraphSkypeForBusinessActivityUserCounts alloc] initWithDictionary:[skypeForBusinessActivityUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```