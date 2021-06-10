---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07b236dc63e463e29709479674b3d4184e2fc1d9
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870589"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards/TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972/endbreak"]]];
[urlRequest setHTTPMethod:@"POST"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

BOOL atAprovedLocation = YES;
payloadDictionary[@"atAprovedLocation"] = atAprovedLocation;

MSGraphItemBody *notes = [[MSGraphItemBody alloc] init];
[notes setContentType: [MSGraphBodyType text]];
[notes setContent:@"end break smaple notes"];
payloadDictionary[@"notes"] = notes;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```