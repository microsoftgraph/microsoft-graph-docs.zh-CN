---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4b1c09e2db5fd2fa2aedd8af4c9d4493e227ad8
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580354"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/68a3e365-f7d9-4a56-b499-24332a9cc572/channels/19:0b50940236084d258c97b21bd01917b0@thread.skype/messages"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphChatMessage *chatMessage = [[MSGraphChatMessage alloc] init];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"<div><div><at id=\"0\">General</at>&nbsp;Hello there!</div></div>"];
[chatMessage setBody:body];
NSMutableArray *mentionsList = [[NSMutableArray alloc] init];
MSGraphChatMessageMention *mentions = [[MSGraphChatMessageMention alloc] init];
[mentions setId: 0];
[mentions setMentionText:@"General"];
MSGraphChatMessageMentionedIdentitySet *mentioned = [[MSGraphChatMessageMentionedIdentitySet alloc] init];
MSGraphTeamworkConversationIdentity *conversation = [[MSGraphTeamworkConversationIdentity alloc] init];
[conversation setId:@"19:0b50940236084d258c97b21bd01917b0@thread.skype"];
[conversation setDisplayName:@"General"];
[conversation setConversationIdentityType: [MSGraphTeamworkConversationIdentityType channel]];
[mentioned setConversation:conversation];
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