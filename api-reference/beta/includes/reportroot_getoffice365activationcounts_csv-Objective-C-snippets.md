---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d9c3021cfad49b239df7316e890e7acaf382e814
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330769"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOffice365ActivationCounts?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *office365ActivationCountsList = [[NSMutableArray alloc] init];
        office365ActivationCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphOffice365ActivationCounts *office365ActivationCounts = [[MSGraphOffice365ActivationCounts alloc] initWithDictionary:[office365ActivationCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```