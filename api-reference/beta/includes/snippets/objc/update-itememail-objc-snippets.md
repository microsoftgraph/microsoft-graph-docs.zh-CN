---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5d1b6a394bea04d73b8580634be4eb2707ba198
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997351"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/emails/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphItemEmail *itemEmail = [[MSGraphItemEmail alloc] init];
[itemEmail setAddress:@"address-value"];
[itemEmail setDisplayName:@"displayName-value"];
[itemEmail setType: [MSGraphEmailType unknown]];

NSError *error;
NSData *itemEmailData = [itemEmail getSerializedDataWithError:&error];
[urlRequest setHTTPBody:itemEmailData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```