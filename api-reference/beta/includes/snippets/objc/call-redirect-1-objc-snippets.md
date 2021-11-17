---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e417c700ce7fbb4dad9b105b76b4b3c88dcc303fbe0f5600b7512ae4b31dbb26
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274202"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/calls/491f0b00-ffff-4bc9-a43e-b226498ec22a/redirect"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *targetsList = [[NSMutableArray alloc] init];
MSGraphInvitationParticipantInfo *targets = [[MSGraphInvitationParticipantInfo alloc] init];
MSGraphIdentitySet *identity = [[MSGraphIdentitySet alloc] init];
MSGraphIdentity *application = [[MSGraphIdentity alloc] init];
[application setDisplayName:@"test bot 2"];
[application setId:@"22bfd41f-550e-477d-8789-f6f7bd2a5e8b"];
[identity setApplication:application];
[targets setIdentity:identity];
[targetsList addObject: targets];
payloadDictionary[@"targets"] = targetsList;

NSString *callbackUri = @"https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039";
payloadDictionary[@"callbackUri"] = callbackUri;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```