---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5cd197dbcc4dedea7d7ab95888b57cc1d1c28f8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945149"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/calls/{id}/participants/invite"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *participantsList = [[NSMutableArray alloc] init];
MSGraphInvitationParticipantInfo *participants = [[MSGraphInvitationParticipantInfo alloc] init];
[participants setReplacesCallId:@"a7ebfb2d-871e-419c-87af-27290b22e8db"];
MSGraphIdentitySet *identity = [[MSGraphIdentitySet alloc] init];
MSGraphIdentity *user = [[MSGraphIdentity alloc] init];
[user setId:@"278405a3-f568-4b3e-b684-009193463064"];
[user setDisplayName:@"string"];
[identity setUser:user];
[participants setIdentity:identity];
[participantsList addObject: participants];
payloadDictionary[@"participants"] = participantsList;

NSString *clientContext = @"f2fa86af-3c51-4bc2-8fc0-475452d9764f";
payloadDictionary[@"clientContext"] = clientContext;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```