---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67f0eb5f3b15ec807c7cbd2a55cac6af91f8182f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335596"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/chats"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphChat *chat = [[MSGraphChat alloc] init];
[chat setChatType: [MSGraphChatType group]];
[chat setTopic:@"Group chat title"];
NSMutableArray *membersList = [[NSMutableArray alloc] init];
MSGraphConversationMember *members = [[MSGraphConversationMember alloc] init];
NSMutableArray *rolesList = [[NSMutableArray alloc] init];
[rolesList addObject: @"owner"];
[members setRoles:rolesList];
[membersList addObject: members];
MSGraphConversationMember *members = [[MSGraphConversationMember alloc] init];
NSMutableArray *rolesList = [[NSMutableArray alloc] init];
[rolesList addObject: @"owner"];
[members setRoles:rolesList];
[membersList addObject: members];
MSGraphConversationMember *members = [[MSGraphConversationMember alloc] init];
NSMutableArray *rolesList = [[NSMutableArray alloc] init];
[rolesList addObject: @"guest"];
[members setRoles:rolesList];
[membersList addObject: members];
[chat setMembers:membersList];

NSError *error;
NSData *chatData = [chat getSerializedDataWithError:&error];
[urlRequest setHTTPBody:chatData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```