---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2ee7e793208d9ba3d996b7b499a540c39bfb21e4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35318547"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/{id}/endpoints"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *endpointList = [[NSMutableArray alloc] init];
        endpointList = [jsonFinal valueForKey:@"value"];
        MSGraphEndpoint *endpoint = [[MSGraphEndpoint alloc] initWithDictionary:[endpointList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```