---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a661a9309f4cb327bdadfb6e9861b709f353ac5b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470981"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphConversation *conversation = [[MSGraphConversation alloc] init];
[conversation setTopic:@"New head count"];
NSMutableArray *threadsList = [[NSMutableArray alloc] init];
MSGraphConversationThread *threads = [[MSGraphConversationThread alloc] init];
NSMutableArray *postsList = [[NSMutableArray alloc] init];
MSGraphPost *posts = [[MSGraphPost alloc] init];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"The confirmation will come by the end of the week."];
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