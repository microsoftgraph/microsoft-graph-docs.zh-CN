---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 432682dd2adf61ec8d0956f63a8873299f630eff
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520097"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants"]]];
[urlRequest setHTTPMethod:@"GET"];
[urlRequest setValue:@"Bearer <TOKEN>" forHTTPHeaderField:@"Authorization"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *ParticipantList = [[NSMutableArray alloc] init];
        ParticipantList = [jsonFinal valueForKey:@"value"];
        MSGraphParticipant *Participant = [[MSGraphParticipant alloc] initWithDictionary:[ParticipantList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```