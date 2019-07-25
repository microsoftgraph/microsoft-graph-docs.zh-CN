---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 99b373805a5fec762740d4b90f614fc71db057b9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709871"
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