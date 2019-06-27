---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 22cb24c203eb20bc7020e05d867b549d7a1ccec2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330214"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/security/tiIndicators"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *tiIndicatorList = [[NSMutableArray alloc] init];
        tiIndicatorList = [jsonFinal valueForKey:@"value"];
        MSGraphTiIndicator *tiIndicator = [[MSGraphTiIndicator alloc] initWithDictionary:[tiIndicatorList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```