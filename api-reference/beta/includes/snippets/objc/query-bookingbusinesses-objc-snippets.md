---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 99b373805a5fec762740d4b90f614fc71db057b9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479371"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses?query=Adventure"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *bookingBusinessList = [[NSMutableArray alloc] init];
        bookingBusinessList = [jsonFinal valueForKey:@"value"];
        MSGraphBookingBusiness *bookingBusiness = [[MSGraphBookingBusiness alloc] initWithDictionary:[bookingBusinessList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```