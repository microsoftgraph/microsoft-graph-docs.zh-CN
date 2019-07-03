---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 056a397e980e0bc042c8d77d75cc0b7ef98bb12b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520325"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365ActiveUserCountsList = [[NSMutableArray alloc] init];
        office365ActiveUserCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365ActiveUserCounts *office365ActiveUserCounts = [[MSGraphOffice365ActiveUserCounts alloc] initWithDictionary:[office365ActiveUserCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```