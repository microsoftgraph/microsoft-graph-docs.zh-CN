---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb3d1455c0fb875ea4d7d65f7e260c61e80585e0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220303"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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

MSGraphIncomingCallOptions *callOptions = [[MSGraphIncomingCallOptions alloc] init];
[callOptions setIsContentSharingNotificationEnabled: true];
payloadDictionary[@"callOptions"] = callOptions;

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