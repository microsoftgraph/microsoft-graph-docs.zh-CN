---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b284d48d5fc1daa9e07e1a709a9c3499b57e480a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718753"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')?$format=text/csv"]]];
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