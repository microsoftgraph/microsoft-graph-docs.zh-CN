---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c895dff31e5222b71c20439b29c2658215e33e60
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727473"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365ActivationsUserCounts?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365ActivationsUserCountsList = [[NSMutableArray alloc] init];
        office365ActivationsUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365ActivationsUserCounts *office365ActivationsUserCounts = [[MSGraphOffice365ActivationsUserCounts alloc] initWithDictionary:[office365ActivationsUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```