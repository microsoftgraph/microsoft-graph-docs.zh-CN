---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c53b34263b43de02c326854b4c3541d062392252
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208290"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/setPresence"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *sessionId = @"22553876-f5ab-4529-bffb-cfe50aa89f87";
payloadDictionary[@"sessionId"] = sessionId;

NSString *availability = @"Available";
payloadDictionary[@"availability"] = availability;

NSString *activity = @"Available";
payloadDictionary[@"activity"] = activity;

NSString *expirationDuration = @"PT1H";
payloadDictionary[@"expirationDuration"] = expirationDuration;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```