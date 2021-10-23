---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25c9c2e00c7ec098822ab1a87785fcde18b3b1fa
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561575"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/calls/{id}/transfer"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphInvitationParticipantInfo *transferTarget = [[MSGraphInvitationParticipantInfo alloc] init];
[transferTarget setEndpointType: [MSGraphEndpointType default]];
MSGraphIdentitySet *identity = [[MSGraphIdentitySet alloc] init];
MSGraphIdentity *user = [[MSGraphIdentity alloc] init];
[user setId:@"550fae72-d251-43ec-868c-373732c2704f"];
[user setTenantId:@"72f988bf-86f1-41af-91ab-2d7cd011db47"];
[user setDisplayName:@"Heidi Steen"];
[identity setUser:user];
[transferTarget setIdentity:identity];
payloadDictionary[@"transferTarget"] = transferTarget;

MSGraphParticipantInfo *transferee = [[MSGraphParticipantInfo alloc] init];
MSGraphIdentitySet *identity = [[MSGraphIdentitySet alloc] init];
MSGraphIdentity *user = [[MSGraphIdentity alloc] init];
[user setId:@"751f6800-3180-414d-bd94-333364659951"];
[user setTenantId:@"72f988bf-86f1-41af-91ab-2d7cd011db47"];
[identity setUser:user];
[transferee setIdentity:identity];
[transferee setParticipantId:@"909c6581-5130-43e9-88f3-fcb3582cde37"];
payloadDictionary[@"transferee"] = transferee;

NSString *languageId = @"languageId-value";
payloadDictionary[@"languageId"] = languageId;

NSString *region = @"region-value";
payloadDictionary[@"region"] = region;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```