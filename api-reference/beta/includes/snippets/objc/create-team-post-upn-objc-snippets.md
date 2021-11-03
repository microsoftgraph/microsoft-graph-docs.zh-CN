---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15b20cd942b7a744a0e55f2791712df620c9dc37
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2021
ms.locfileid: "60672009"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTeam *team = [[MSGraphTeam alloc] init];
[team setDisplayName:@"My Sample Team"];
[team setDescription:@"My Sample Team’s Description"];
NSMutableArray *membersList = [[NSMutableArray alloc] init];
MSGraphConversationMember *members = [[MSGraphConversationMember alloc] init];
NSMutableArray *rolesList = [[NSMutableArray alloc] init];
[rolesList addObject: @"owner"];
[members setRoles:rolesList];
[membersList addObject: members];
[team setMembers:membersList];

NSError *error;
NSData *teamData = [team getSerializedDataWithError:&error];
[urlRequest setHTTPBody:teamData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```