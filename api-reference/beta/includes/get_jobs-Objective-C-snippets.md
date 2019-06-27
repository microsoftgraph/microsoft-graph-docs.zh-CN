---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ec670f06fef7e2130e2d0bf04f520ae4237db461
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330448"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/synchronization/jobs/"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *synchronizationJobList = [[NSMutableArray alloc] init];
        synchronizationJobList = [jsonFinal valueForKey:@"value"];
        MSGraphSynchronizationJob *synchronizationJob = [[MSGraphSynchronizationJob alloc] initWithDictionary:[synchronizationJobList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```