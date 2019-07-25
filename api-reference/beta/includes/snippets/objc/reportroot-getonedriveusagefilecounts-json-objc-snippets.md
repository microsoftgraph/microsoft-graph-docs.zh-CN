---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c21055ed9ab58004c5142e91442641b94e9d1e80
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719133"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOneDriveUsageFileCounts(period='D7')?$format=application/json"]]];
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