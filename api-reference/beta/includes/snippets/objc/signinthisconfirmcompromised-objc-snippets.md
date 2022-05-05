---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c78113dbe4c234bbb0bca4fadc049ae125e5774b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212816"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/auditLogs/signIns/confirmCompromised"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *requestIdsList = [[NSMutableArray alloc] init];
[requestIdsList addObject: @"f01c6af6-6683-4a37-a945-0a925501eede"];
[requestIdsList addObject: @"42bf60ac-d0cb-4206-aa5c-101884298f55"];
[requestIdsList addObject: @"f09c8f14-8d8e-42cf-8a7e-732b0594e79b"];
payloadDictionary[@"requestIds"] = requestIdsList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```