---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 32627705c8d5f98d28f6629249e3e599f2972a29
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874165"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getCredentialUsageSummary(period='D30')?$filter=feature%20eq%20'registration'"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *credentialUsageSummaryList = [[NSMutableArray alloc] init];
        credentialUsageSummaryList = [jsonFinal valueForKey:@"value"];
        MSGraphCredentialUsageSummary *credentialUsageSummary = [[MSGraphCredentialUsageSummary alloc] initWithDictionary:[credentialUsageSummaryList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```