---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a1a7556b3f875ccd3cde2ef19cd8e04a4908b62
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871133"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/answer"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *callbackUri = @"https://bot.contoso.com/api/calls";
payloadDictionary[@"callbackUri"] = callbackUri;

NSMutableArray *acceptedModalitiesList = [[NSMutableArray alloc] init];
[acceptedModalitiesList addObject: @"audio"];
payloadDictionary[@"acceptedModalities"] = acceptedModalitiesList;

MSGraphMediaConfig *mediaConfig = [[MSGraphMediaConfig alloc] init];
[mediaConfig setBlob:@"<Media Session Configuration Blob>"];
payloadDictionary[@"mediaConfig"] = mediaConfig;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```