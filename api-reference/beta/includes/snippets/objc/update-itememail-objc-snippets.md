---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9097d909e854336096ba48bc7d91b6143c62bebd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774325"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{userId}/profile/emails/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphItemEmail *itemEmail = [[MSGraphItemEmail alloc] init];
[itemEmail setDisplayName:@"Business Email"];
[itemEmail setType: [MSGraphEmailType work]];

NSError *error;
NSData *itemEmailData = [itemEmail getSerializedDataWithError:&error];
[urlRequest setHTTPBody:itemEmailData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```