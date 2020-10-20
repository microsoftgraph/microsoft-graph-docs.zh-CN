---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b11041c099023825e3071ed04f3b675ba420bf08
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620965"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{id}/channels/{id}/messages"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphChatMessage *chatMessage = [[MSGraphChatMessage alloc] init];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContent:@"Hello world"];
[chatMessage setBody:body];

NSError *error;
NSData *chatMessageData = [chatMessage getSerializedDataWithError:&error];
[urlRequest setHTTPBody:chatMessageData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```