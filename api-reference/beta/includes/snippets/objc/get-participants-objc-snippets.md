---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62e1d6abc7958d02709b723f186c97626eab8ade
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302397"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *participantList = [[NSMutableArray alloc] init];
        participantList = [jsonFinal valueForKey:@"value"];
        MSGraphParticipant *participant = [[MSGraphParticipant alloc] initWithDictionary:[participantList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```