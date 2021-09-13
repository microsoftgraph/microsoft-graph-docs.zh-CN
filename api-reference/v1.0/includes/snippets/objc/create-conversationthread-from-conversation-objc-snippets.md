---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e34be0522c749dac31b608d8e9006f81ae78d8ce
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068268"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/{id}/conversations/{id}/threads"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphConversationThread *conversationThread = [[MSGraphConversationThread alloc] init];
[conversationThread setTopic:@"Take your wellness days and rest"];
NSMutableArray *postsList = [[NSMutableArray alloc] init];
MSGraphPost *posts = [[MSGraphPost alloc] init];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"Waiting for the summer holidays."];
[posts setBody:body];
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