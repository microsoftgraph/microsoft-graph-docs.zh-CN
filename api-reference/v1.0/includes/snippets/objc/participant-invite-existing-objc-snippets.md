---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7be0e1b4bb99e6fe443ea1c28b9c74ad0b10e6e2
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865820"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/calls/ab6233a5-20b7-4c5e-bea2-ce56c9776429/participants/invite"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *participantsList = [[NSMutableArray alloc] init];
MSGraphInvitationParticipantInfo *participants = [[MSGraphInvitationParticipantInfo alloc] init];
[participants setReplacesCallId:@"a7ebfb2d-871e-419c-87af-27290b22e8db"];
MSGraphIdentitySet *identity = [[MSGraphIdentitySet alloc] init];
MSGraphIdentity *user = [[MSGraphIdentity alloc] init];
[user setId:@"7e1b4346-85a6-4bdd-abe3-d11c5d420efe"];
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