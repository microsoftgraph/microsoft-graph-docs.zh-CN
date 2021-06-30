---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 633d5665a47f5b0f44a10f19e39a5e6720244af0
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207562"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages"]]];
[urlRequest setHTTPMethod:@"POST"];

MSGraphChatMessage *chatMessage = [[MSGraphChatMessage alloc] init];
[chatMessage setCreatedDateTime: "2019-02-04T19:58:15.511Z"];
MSGraphChatMessageFromIdentitySet *from = [[MSGraphChatMessageFromIdentitySet alloc] init];
MSGraphIdentity *user = [[MSGraphIdentity alloc] init];
[user setId:@"id-value"];
[user setDisplayName:@"Joh Doe"];
[user setUserIdentityType: [MSGraphTeamworkUserIdentityType aadUser]];
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