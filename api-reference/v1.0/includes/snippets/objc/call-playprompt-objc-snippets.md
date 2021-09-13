---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bcd303465838ef038a8aff1bfe0b8416ce5830df80920782e9b8c99864f2d00d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279698"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *clientContext = @"d45324c1-fcb5-430a-902c-f20af696537c";
payloadDictionary[@"clientContext"] = clientContext;

NSMutableArray *promptsList = [[NSMutableArray alloc] init];
MSGraphPrompt *prompts = [[MSGraphPrompt alloc] init];
MSGraphMediaInfo *mediaInfo = [[MSGraphMediaInfo alloc] init];
[mediaInfo setUri:@"https://cdn.contoso.com/beep.wav"];
[mediaInfo setResourceId:@"1D6DE2D4-CD51-4309-8DAA-70768651088E"];
[prompts setMediaInfo:mediaInfo];
[promptsList addObject: prompts];
payloadDictionary[@"prompts"] = promptsList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```