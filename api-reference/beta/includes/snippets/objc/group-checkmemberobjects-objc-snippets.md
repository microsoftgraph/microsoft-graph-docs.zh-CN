---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b434773e256890f4cfbbf515224259491b852ee0
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041801"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/{id}/checkMemberObjects"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *idsList = [[NSMutableArray alloc] init];
[idsList addObject: @"80a963dd-84af-4eb8-b2a6-781e444d4fb0"];
[idsList addObject: @"62e90394-69f5-4237-9190-012177145e10"];
[idsList addObject: @"86a64f51-3a64-4cc6-a8c8-6b8f000c0f52"];
[idsList addObject: @"ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"];
payloadDictionary[@"ids"] = idsList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```