---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0e9022635178cd1a2e212bc65053d38eaae15472
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499943"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessParticipantActivityUserCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessParticipantActivityUserCountsList = [[NSMutableArray alloc] init];
        skypeForBusinessParticipantActivityUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessParticipantActivityUserCounts *skypeForBusinessParticipantActivityUserCounts = [[MSGraphSkypeForBusinessParticipantActivityUserCounts alloc] initWithDictionary:[skypeForBusinessParticipantActivityUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```