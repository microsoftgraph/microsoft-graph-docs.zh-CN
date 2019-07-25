---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c0e64a8a5d49d12a21acbedad012b7653675594e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727089"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSharePointActivityPages(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *sharePointActivityPagesList = [[NSMutableArray alloc] init];
        sharePointActivityPagesList = [jsonFinal valueForKey:@"value"];
        MSGraphSharePointActivityPages *sharePointActivityPages = [[MSGraphSharePointActivityPages alloc] initWithDictionary:[sharePointActivityPagesList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```