---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6462533a25783c52f3dcfe5ad1cea0afda5e7b3f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719134"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOneDriveUsageFileCounts(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *oneDriveUsageFileCountsList = [[NSMutableArray alloc] init];
        oneDriveUsageFileCountsList = [jsonFinal valueForKey:@"value"];
        MSGraphOneDriveUsageFileCounts *oneDriveUsageFileCounts = [[MSGraphOneDriveUsageFileCounts alloc] initWithDictionary:[oneDriveUsageFileCountsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```