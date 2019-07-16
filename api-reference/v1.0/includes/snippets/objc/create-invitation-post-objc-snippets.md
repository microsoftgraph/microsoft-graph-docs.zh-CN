---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7532072da9d597a5d49388a8f6a145e96f82c11b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738735"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/invitations"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphInvitation *invitation = [[MSGraphInvitation alloc] init];
[invitation setInvitedUserEmailAddress:@"yyy@test.com"];
[invitation setInviteRedirectUrl:@"https://myapp.com"];

NSError *error;
NSData *invitationData = [invitation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:invitationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```