---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8bd4060c7817cde9536b7647962c4c8546e8f86
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681600"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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

BOOL loop = NO;
payloadDictionary[@"loop"] = loop;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```