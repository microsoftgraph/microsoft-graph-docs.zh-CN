---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5d7cbfee29f646c0166811770254f63998eab5f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777781"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{userId}/profile/patents/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphItemPatent *itemPatent = [[MSGraphItemPatent alloc] init];
[itemPatent setNumber:@"USPTO-3954432633"];
[itemPatent setWebUrl:@"https://patents.gov/3954432633"];

NSError *error;
NSData *itemPatentData = [itemPatent getSerializedDataWithError:&error];
[urlRequest setHTTPBody:itemPatentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```