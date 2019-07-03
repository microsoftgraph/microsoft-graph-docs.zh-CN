---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 72f12086f46d6ae238b72da03c12c7887ad2d526
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520919"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365GroupsActivityDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365GroupsActivityDetailList = [[NSMutableArray alloc] init];
        office365GroupsActivityDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365GroupsActivityDetail *office365GroupsActivityDetail = [[MSGraphOffice365GroupsActivityDetail alloc] initWithDictionary:[office365GroupsActivityDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```