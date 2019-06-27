---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d9b6c69817ddcfadfd31bb3891b1d9c3f06f8601
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330374"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingCurrencies"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *bookingCurrencyList = [[NSMutableArray alloc] init];
        bookingCurrencyList = [jsonFinal valueForKey:@"value"];
        MSGraphBookingCurrency *bookingCurrency = [[MSGraphBookingCurrency alloc] initWithDictionary:[bookingCurrencyList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```