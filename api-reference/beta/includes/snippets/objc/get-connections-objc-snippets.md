---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29e945fa823d527164d86ef1db1559ce9d1778d0
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994640"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/external/connections"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *externalConnectionList = [[NSMutableArray alloc] init];
        externalConnectionList = [jsonFinal valueForKey:@"value"];
        MSGraphExternalConnection *externalConnection = [[MSGraphExternalConnection alloc] initWithDictionary:[externalConnectionList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```