---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 49b2b48a7489e7c8878fb3da7b871219a4301d84
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479212"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessOrganizerActivityUserCountsList = [[NSMutableArray alloc] init];
        skypeForBusinessOrganizerActivityUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessOrganizerActivityUserCounts *skypeForBusinessOrganizerActivityUserCounts = [[MSGraphSkypeForBusinessOrganizerActivityUserCounts alloc] initWithDictionary:[skypeForBusinessOrganizerActivityUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```