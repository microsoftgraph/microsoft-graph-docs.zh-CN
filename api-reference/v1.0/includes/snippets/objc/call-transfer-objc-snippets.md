---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 563d0e706679fdd1e70c3acf19b5c5c98a8f185b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865833"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/calls/{id}/transfer"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphInvitationParticipantInfo *transferTarget = [[MSGraphInvitationParticipantInfo alloc] init];
[transferTarget setEndpointType:@"default"];
MSGraphIdentitySet *identity = [[MSGraphIdentitySet alloc] init];
MSGraphIdentity *user = [[MSGraphIdentity alloc] init];
[user setId:@"550fae72-d251-43ec-868c-373732c2704f"];
[user setDisplayName:@"Heidi Steen"];
[identity setUser:user];
[transferTarget setIdentity:identity];
[transferTarget setReplacesCallId:@"replacesCallId-value"];
payloadDictionary[@"transferTarget"] = transferTarget;

NSString *clientContext = @"9e90d1c1-f61e-43e7-9f75-d420159aae08";
payloadDictionary[@"clientContext"] = clientContext;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```