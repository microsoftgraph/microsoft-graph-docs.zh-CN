---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0adea98d2d57bb510af75d963a1748b62e71cd8
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581313"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphConversationMember *conversationMember = [[MSGraphConversationMember alloc] init];
[conversationMember setVisibleHistoryStartDateTime: "0001-01-01T00:00:00Z"];
NSMutableArray *rolesList = [[NSMutableArray alloc] init];
[rolesList addObject: @"owner"];
[conversationMember setRoles:rolesList];

NSError *error;
NSData *conversationMemberData = [conversationMember getSerializedDataWithError:&error];
[urlRequest setHTTPBody:conversationMemberData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```