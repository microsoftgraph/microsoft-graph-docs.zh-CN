---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 147f884de7e9c33e0b6af1404d95f0f24d359fb4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35318220"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/{id}/threads"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphConversationThread *conversationThread = [[MSGraphConversationThread alloc] init];
[conversationThread setTopic:@"New Conversation Thread Topic"];
NSMutableArray *postsList = [[NSMutableArray alloc] init];
MSGraphPost *posts = [[MSGraphPost alloc] init];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"this is body content"];
[posts setBody:body];
NSMutableArray *newParticipantsList = [[NSMutableArray alloc] init];
MSGraphRecipient *newParticipants = [[MSGraphRecipient alloc] init];
MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] init];
[emailAddress setName:@"Alex Darrow"];
[emailAddress setAddress:@"alexd@contoso.com"];
[newParticipants setEmailAddress:emailAddress];
[newParticipantsList addObject: newParticipants];
[posts setNewParticipants:newParticipantsList];
[postsList addObject: posts];
[conversationThread setPosts:postsList];

NSError *error;
NSData *conversationThreadData = [conversationThread getSerializedDataWithError:&error];
[urlRequest setHTTPBody:conversationThreadData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```