---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f7716ce36f7d1faf349e91ac92046ae47767dbf9abe45abb4fe699f4bfe57e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218957"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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