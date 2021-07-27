---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e77cfa4f1483feac1d6fc5fd5e1c0b508be3dbc1
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581510"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/calls/{id}/answer"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *callbackUri = @"callbackUri-value";
payloadDictionary[@"callbackUri"] = callbackUri;

MSGraphMediaConfig *mediaConfig = [[MSGraphMediaConfig alloc] init];
[mediaConfig setBlob:@"<Media Session Configuration Blob>"];
payloadDictionary[@"mediaConfig"] = mediaConfig;

NSMutableArray *acceptedModalitiesList = [[NSMutableArray alloc] init];
[acceptedModalitiesList addObject: @"audio"];
payloadDictionary[@"acceptedModalities"] = acceptedModalitiesList;

int32_t participantCapacity = 200;
payloadDictionary[@"participantCapacity"] = participantCapacity;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```