---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 13c365fc2616806673f6987e629462014684202c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727639"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getEmailAppUsageUserCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *emailAppUsageUserCountsList = [[NSMutableArray alloc] init];
        emailAppUsageUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphEmailAppUsageUserCounts *emailAppUsageUserCounts = [[MSGraphEmailAppUsageUserCounts alloc] initWithDictionary:[emailAppUsageUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```