---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fa83d7c3b864d542af37478699aeb3a10b18cf1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022402"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphConversation *conversation = [[MSGraphConversation alloc] init];
[conversation setTopic:@"Take your wellness days and rest"];
NSMutableArray *threadsList = [[NSMutableArray alloc] init];
MSGraphConversationThread *threads = [[MSGraphConversationThread alloc] init];
NSMutableArray *postsList = [[NSMutableArray alloc] init];
MSGraphPost *posts = [[MSGraphPost alloc] init];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"Contoso cares about you: Rest and Recharge"];
[posts setBody:body];
NSMutableArray *newParticipantsList = [[NSMutableArray alloc] init];
MSGraphRecipient *newParticipants = [[MSGraphRecipient alloc] init];
MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] init];
[emailAddress setName:@"Adele Vance"];
[emailAddress setAddress:@"AdeleV@contoso.onmicrosoft.com"];
[newParticipants setEmailAddress:emailAddress];
[newParticipantsList addObject: newParticipants];
[posts setNewParticipants:newParticipantsList];
[postsList addObject: posts];
[threads setPosts:postsList];
[threadsList addObject: threads];
[conversation setThreads:threadsList];

NSError *error;
NSData *conversationData = [conversation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:conversationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```