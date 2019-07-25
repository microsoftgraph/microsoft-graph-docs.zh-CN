---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 745ac0280a8e463b25e6ce94b3a657d4afd89d70
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726296"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getYammerGroupsActivityCounts(period='D7')?$format=application/json"]]];
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