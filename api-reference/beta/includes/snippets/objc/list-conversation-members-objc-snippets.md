---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd0191dc883b944b2d8e86a3997a0ef2fba704d6
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633347"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/chats/{id}/members"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *conversationMemberList = [[NSMutableArray alloc] init];
        conversationMemberList = [jsonFinal valueForKey:@"value"];
        MSGraphConversationMember *conversationMember = [[MSGraphConversationMember alloc] initWithDictionary:[conversationMemberList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```