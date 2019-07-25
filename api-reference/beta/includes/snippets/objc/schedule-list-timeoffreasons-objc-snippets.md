---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4e7c5367257e0c66cf971fa7580013ba80077d74
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718194"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{teamId}/schedule/timeOffReasons"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *timeOffReasonList = [[NSMutableArray alloc] init];
        timeOffReasonList = [jsonFinal valueForKey:@"value"];
        MSGraphTimeOffReason *timeOffReason = [[MSGraphTimeOffReason alloc] initWithDictionary:[timeOffReasonList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```