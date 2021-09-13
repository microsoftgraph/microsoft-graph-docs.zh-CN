---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84e22a68ab1c09d17022097e9e23b75bdd02fe287cb870efcf4d22f9b4df623f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163272"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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