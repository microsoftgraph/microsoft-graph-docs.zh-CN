---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 830433708aa6ba8a294c0894a0fd909ff16b941f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330714"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *oneDriveUsageAccountCountsList = [[NSMutableArray alloc] init];
        oneDriveUsageAccountCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphOneDriveUsageAccountCounts *oneDriveUsageAccountCounts = [[MSGraphOneDriveUsageAccountCounts alloc] initWithDictionary:[oneDriveUsageAccountCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```