---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 23c4de516564c48267e054634cc3996d03c21088
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330067"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getEmailAppUsageUserDetail(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *emailAppUsageUserDetailList = [[NSMutableArray alloc] init];
        emailAppUsageUserDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphEmailAppUsageUserDetail *emailAppUsageUserDetail = [[MSGraphEmailAppUsageUserDetail alloc] initWithDictionary:[emailAppUsageUserDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```