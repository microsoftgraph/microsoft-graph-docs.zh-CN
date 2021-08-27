---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 146d3bcca325d98494562aeaa79a8237c1946830464539b73b4ff10cc75067c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409179"
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
[body setContent:@"<div><div><at id=\"0\">GraphTesting</at>&nbsp;Hello team</div></div>"];
[chatMessage setBody:body];
NSMutableArray *mentionsList = [[NSMutableArray alloc] init];
MSGraphChatMessageMention *mentions = [[MSGraphChatMessageMention alloc] init];
[mentions setId: 0];
[mentions setMentionText:@"GraphTesting"];
MSGraphChatMessageMentionedIdentitySet *mentioned = [[MSGraphChatMessageMentionedIdentitySet alloc] init];
MSGraphTeamworkConversationIdentity *conversation = [[MSGraphTeamworkConversationIdentity alloc] init];
[conversation setId:@"68a3e365-f7d9-4a56-b499-24332a9cc572"];
[conversation setDisplayName:@"GraphTesting"];
[conversation setConversationIdentityType: [MSGraphTeamworkConversationIdentityType team]];
[mentioned setConversation:conversation];
[mentions setMentioned:mentioned];
[mentionsList addObject: mentions];
[chatMessage setMentions:mentionsList];
NSMutableArray *reactionsList = [[NSMutableArray alloc] init];
[chatMessage setReactions:reactionsList];

NSError *error;
NSData *chatMessageData = [chatMessage getSerializedDataWithError:&error];
[urlRequest setHTTPBody:chatMessageData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```