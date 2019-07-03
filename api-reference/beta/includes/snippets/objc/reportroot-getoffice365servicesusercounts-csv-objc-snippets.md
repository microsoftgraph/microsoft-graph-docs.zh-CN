---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4dbeae6a23eb12d63ca0b807817bd2b0c820010f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500648"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365ServicesUserCountsList = [[NSMutableArray alloc] init];
        office365ServicesUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365ServicesUserCounts *office365ServicesUserCounts = [[MSGraphOffice365ServicesUserCounts alloc] initWithDictionary:[office365ServicesUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```