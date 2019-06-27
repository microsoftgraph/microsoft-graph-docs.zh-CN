---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f269befa443d26c7c14183c9aba1f84616cf538e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330385"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/synchronization/jobs/{jobId}/restart"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"Bearer <token>" forHTTPHeaderField:@"Authorization"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphSynchronizationJobRestartCriteria *criteria = [[MSGraphSynchronizationJobRestartCriteria alloc] init];
[criteria setResetScope: [MSGraphSynchronizationJobRestartScope ConnectorDataStore]];
payloadDictionary[@"criteria"] = criteria;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```