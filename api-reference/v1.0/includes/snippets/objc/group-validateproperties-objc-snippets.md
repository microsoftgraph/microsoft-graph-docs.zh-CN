---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8055de62a3fe0c83025cae19ae2683487600a5913bb8257fe8ed8892a4a68dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409554"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/{id}/validateProperties"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *displayName = @"Myprefix_test_mysuffix";
payloadDictionary[@"displayName"] = displayName;

NSString *mailNickname = @"Myprefix_test_mysuffix";
payloadDictionary[@"mailNickname"] = mailNickname;

NSString *onBehalfOfUserId = @"onBehalfOfUserId-value";
payloadDictionary[@"onBehalfOfUserId"] = onBehalfOfUserId;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```