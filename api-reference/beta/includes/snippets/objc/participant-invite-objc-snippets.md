---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ed4304276c2bf70a24f81d6b759812e292fe05ce
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730553"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/app/calls/{id}/participants/invite"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *participantsList = [[NSMutableArray alloc] init];
MSGraphInvitationParticipantInfo *participants = [[MSGraphInvitationParticipantInfo alloc] init];
[participants setEndpointType: [MSGraphEndpointType Default]];
MSGraphIdentitySet *identity = [[MSGraphIdentitySet alloc] init];
MSGraphIdentity *user = [[MSGraphIdentity alloc] init];
[user setId:@"550fae72-d251-43ec-868c-373732c2704f"];
[user setTenantId:@"72f988bf-86f1-41af-91ab-2d7cd011db47"];
[user setDisplayName:@"Heidi Steen"];
[identity setUser:user];
[participants setIdentity:identity];
[participants setLanguageId:@"languageId-value"];
[participants setRegion:@"region-value"];
[participants setReplacesCallId:@"replacesCallId-value"];
[participantsList addObject: participants];
payloadDictionary[@"participants"] = participantsList;

NSString *clientContext = @"clientContext-value";
payloadDictionary[@"clientContext"] = clientContext;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```