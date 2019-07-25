---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c18044cc6289551d316dfb7d89f2069371a1c75e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718799"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessDeviceUsageUserDetailList = [[NSMutableArray alloc] init];
        skypeForBusinessDeviceUsageUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessDeviceUsageUserDetail *skypeForBusinessDeviceUsageUserDetail = [[MSGraphSkypeForBusinessDeviceUsageUserDetail alloc] initWithDictionary:[skypeForBusinessDeviceUsageUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```