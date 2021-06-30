---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e74a014b1c0f32f081bd269e2590026b5ca5818a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210033"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTeamworkTag *teamworkTag = [[MSGraphTeamworkTag alloc] init];
[teamworkTag setDisplayName:@"Finance"];
NSMutableArray *membersList = [[NSMutableArray alloc] init];
MSGraphTeamworkTagMember *members = [[MSGraphTeamworkTagMember alloc] init];
[members setUserId:@"92f6952f-61ca-4a94-8910-508a240bc167"];
[membersList addObject: members];
MSGraphTeamworkTagMember *members = [[MSGraphTeamworkTagMember alloc] init];
[members setUserId:@"085d800c-b86b-4bfc-a857-9371ad1caf29"];
[membersList addObject: members];
[teamworkTag setMembers:membersList];

NSError *error;
NSData *teamworkTagData = [teamworkTag getSerializedDataWithError:&error];
[urlRequest setHTTPBody:teamworkTagData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```