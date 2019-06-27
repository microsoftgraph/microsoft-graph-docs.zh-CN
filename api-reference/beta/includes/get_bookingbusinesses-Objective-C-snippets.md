---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 83b780919333f8e6ecf858943b691dcca47e02bd
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330375"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses"]]];
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