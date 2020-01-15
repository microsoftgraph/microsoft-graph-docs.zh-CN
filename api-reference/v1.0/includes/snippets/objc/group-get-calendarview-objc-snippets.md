---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5412847f0c5efdfcc3a17ae39d3aadb50e34e4d9
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41123115"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-10-01T19:00:00.00-08:00"]]];
[urlRequest setHTTPMethod:@"GET"];
[urlRequest setValue:@"outlook.body-content-type=\"text\"" forHTTPHeaderField:@"Prefer"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *eventList = [[NSMutableArray alloc] init];
        eventList = [jsonFinal valueForKey:@"value"];
        MSGraphEvent *event = [[MSGraphEvent alloc] initWithDictionary:[eventList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```