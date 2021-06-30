---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdcb18e3761c8a7829781049a6209858fdd4be9b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211890"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages/1590776551682/replies"]]];
[urlRequest setHTTPMethod:@"POST"];

MSGraphChatMessage *chatMessage = [[MSGraphChatMessage alloc] init];
[chatMessage setCreatedDateTime: "2019-02-04T19:58:15.511Z"];
MSGraphChatMessageFromIdentitySet *from = [[MSGraphChatMessageFromIdentitySet alloc] init];
MSGraphIdentity *user = [[MSGraphIdentity alloc] init];
[user setId:@"8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca"];
[user setDisplayName:@"John Doe"];
[from setUser:user];
[chatMessage setFrom:from];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"Hello World"];
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