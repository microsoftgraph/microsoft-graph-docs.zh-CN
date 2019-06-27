---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 253758f714d3cf5a5be27bdd6080746e47e4d952
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330733"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365ActiveUserDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365ActiveUserDetailList = [[NSMutableArray alloc] init];
        office365ActiveUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365ActiveUserDetail *office365ActiveUserDetail = [[MSGraphOffice365ActiveUserDetail alloc] initWithDictionary:[office365ActiveUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```