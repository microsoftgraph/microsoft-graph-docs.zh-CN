---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 122cc35d31b840b1af209bb3459cfe82adb646d6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719332"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365GroupsActivityGroupCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365GroupsActivityGroupCountsList = [[NSMutableArray alloc] init];
        office365GroupsActivityGroupCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365GroupsActivityGroupCounts *office365GroupsActivityGroupCounts = [[MSGraphOffice365GroupsActivityGroupCounts alloc] initWithDictionary:[office365GroupsActivityGroupCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```