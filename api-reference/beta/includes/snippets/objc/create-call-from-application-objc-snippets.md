---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da4022c52fcf3856088ec7bc81bc062768afa4ff
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "38000173"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/app/calls"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"Bearer <Token>" forHTTPHeaderField:@"Authorization"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCall *call = [[MSGraphCall alloc] init];
[call setCallbackUri:@"https://bot.contoso.com/callback"];
NSMutableArray *targetsList = [[NSMutableArray alloc] init];
MSGraphInvitationParticipantInfo *targets = [[MSGraphInvitationParticipantInfo alloc] init];
MSGraphIdentitySet *identity = [[MSGraphIdentitySet alloc] init];
MSGraphIdentity *user = [[MSGraphIdentity alloc] init];
[user setDisplayName:@"John"];
[user setId:@"112f7296-5fa4-42ca-bae8-6a692b15d4b8"];
[identity setUser:user];
[targets setIdentity:identity];
[targetsList addObject: targets];
[call setTargets:targetsList];
NSMutableArray *requestedModalitiesList = [[NSMutableArray alloc] init];
[requestedModalitiesList addObject: @"audio"];
[call setRequestedModalities:requestedModalitiesList];
MSGraphMediaConfig *mediaConfig = [[MSGraphMediaConfig alloc] init];
[call setMediaConfig:mediaConfig];

NSError *error;
NSData *callData = [call getSerializedDataWithError:&error];
[urlRequest setHTTPBody:callData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```