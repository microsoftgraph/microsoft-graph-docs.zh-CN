---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e1433cf43a22e8f3354c05744d25c5b313933cde
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330797"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getSkypeForBusinessActivityUserDetail(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *skypeForBusinessActivityUserDetailList = [[NSMutableArray alloc] init];
        skypeForBusinessActivityUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphSkypeForBusinessActivityUserDetail *skypeForBusinessActivityUserDetail = [[MSGraphSkypeForBusinessActivityUserDetail alloc] initWithDictionary:[skypeForBusinessActivityUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```