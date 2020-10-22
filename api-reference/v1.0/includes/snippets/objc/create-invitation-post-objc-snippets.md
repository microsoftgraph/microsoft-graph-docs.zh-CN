---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6eef782c71bfa535ff327dbe9126fa09ba06ef6
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635760"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/invitations"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphInvitation *invitation = [[MSGraphInvitation alloc] init];
[invitation setInvitedUserEmailAddress:@"yyy@test.com"];
[invitation setInviteRedirectUrl:@"https://myapp.contoso.com"];

NSError *error;
NSData *invitationData = [invitation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:invitationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```