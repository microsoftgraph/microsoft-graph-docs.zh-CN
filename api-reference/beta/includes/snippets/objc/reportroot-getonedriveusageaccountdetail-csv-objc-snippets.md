---
description: 自动生成的文件。 不修改
ms.openlocfilehash: beab66b15a04f70f8f3c53b9afd5dab1ce77cabd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727174"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *oneDriveUsageAccountDetailList = [[NSMutableArray alloc] init];
        oneDriveUsageAccountDetailList = [jsonFinal valueForKey:@"value"];
        MSGraphOneDriveUsageAccountDetail *oneDriveUsageAccountDetail = [[MSGraphOneDriveUsageAccountDetail alloc] initWithDictionary:[oneDriveUsageAccountDetailList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```