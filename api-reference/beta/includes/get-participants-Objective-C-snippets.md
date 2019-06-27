---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 432682dd2adf61ec8d0956f63a8873299f630eff
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35315671"
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