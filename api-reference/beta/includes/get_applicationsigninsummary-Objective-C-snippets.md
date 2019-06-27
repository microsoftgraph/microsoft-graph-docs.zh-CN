---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1d698317114a610e72ccb6b01556205dd3f316fb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330393"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getAzureADApplicationSignInSummary(period='D7')"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *applicationSignInSummaryList = [[NSMutableArray alloc] init];
        applicationSignInSummaryList = [jsonFinal valueForKey:@"value"];
        MSGraphApplicationSignInSummary *applicationSignInSummary = [[MSGraphApplicationSignInSummary alloc] initWithDictionary:[applicationSignInSummaryList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```