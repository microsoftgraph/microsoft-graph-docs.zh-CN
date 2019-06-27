---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 05ebbb59d4d3387f5e13e5a57a6b8f277fa25d6f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35314547"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/subscribedSkus"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *subscribedSkuList = [[NSMutableArray alloc] init];
        subscribedSkuList = [jsonFinal valueForKey:@"value"];
        MSGraphSubscribedSku *subscribedSku = [[MSGraphSubscribedSku alloc] initWithDictionary:[subscribedSkuList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```