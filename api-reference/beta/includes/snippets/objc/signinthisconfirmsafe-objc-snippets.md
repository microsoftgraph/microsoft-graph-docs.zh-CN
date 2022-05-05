---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24e8b07f094769ff1fc128ff247010fb78e8d2f8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212724"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/auditLogs/signIns/confirmSafe"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *requestIdsList = [[NSMutableArray alloc] init];
[requestIdsList addObject: @"5a0c76d2-cb57-4ece-9bc1-c323178f116a"];
[requestIdsList addObject: @"96609214-09ef-4f80-9d4a-ace5fceecaec"];
[requestIdsList addObject: @"05020696-4eb8-45a3-918f-8f8bb7ad6015"];
payloadDictionary[@"requestIds"] = requestIdsList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```