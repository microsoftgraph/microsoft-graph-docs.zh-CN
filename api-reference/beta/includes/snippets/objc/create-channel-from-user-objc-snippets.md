---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a58c3a68a880f41f011eed4a2802b7ad92e9b0ca
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402277"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{group_id}/channels"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphChannel *channel = [[MSGraphChannel alloc] init];
[channel setMembershipType: [MSGraphChannelMembershipType private]];
[channel setDisplayName:@"My First Private Channel"];
[channel setDescription:@"This is my first private channels"];
NSMutableArray *membersList = [[NSMutableArray alloc] init];
MSGraphConversationMember *members = [[MSGraphConversationMember alloc] init];
NSMutableArray *rolesList = [[NSMutableArray alloc] init];
[rolesList addObject: @"owner"];
[members setRoles:rolesList];
[membersList addObject: members];
[channel setMembers:membersList];

NSError *error;
NSData *channelData = [channel getSerializedDataWithError:&error];
[urlRequest setHTTPBody:channelData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```