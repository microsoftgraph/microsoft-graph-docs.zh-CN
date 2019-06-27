---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 056a397e980e0bc042c8d77d75cc0b7ef98bb12b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35329809"
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