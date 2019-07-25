---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a8ac2b3480e8767fcc72ee52f4e4421716f8a50b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719609"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getEmailAppUsageUserDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *emailAppUsageUserDetailList = [[NSMutableArray alloc] init];
        emailAppUsageUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphEmailAppUsageUserDetail *emailAppUsageUserDetail = [[MSGraphEmailAppUsageUserDetail alloc] initWithDictionary:[emailAppUsageUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```