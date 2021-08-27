---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b7f267592554d2ebb0005ec07e303b5c1ae4459735afad3c644c38b51110f16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106964"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphChatMessage *chatMessage = [[MSGraphChatMessage alloc] init];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"Hello World <at id=\"0\">Jane Smith</at>"];
[chatMessage setBody:body];
NSMutableArray *mentionsList = [[NSMutableArray alloc] init];
MSGraphChatMessageMention *mentions = [[MSGraphChatMessageMention alloc] init];
[mentions setId: 0];
[mentions setMentionText:@"Jane Smith"];
MSGraphChatMessageMentionedIdentitySet *mentioned = [[MSGraphChatMessageMentionedIdentitySet alloc] init];
MSGraphIdentity *user = [[MSGraphIdentity alloc] init];
[user setDisplayName:@"Jane Smith"];
[user setId:@"ef1c916a-3135-4417-ba27-8eb7bd084193"];
[user setUserIdentityType: [MSGraphTeamworkUserIdentityType aadUser]];
[mentioned setUser:user];
[mentions setMentioned:mentioned];
[mentionsList addObject: mentions];
[chatMessage setMentions:mentionsList];

NSError *error;
NSData *chatMessageData = [chatMessage getSerializedDataWithError:&error];
[urlRequest setHTTPBody:chatMessageData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```