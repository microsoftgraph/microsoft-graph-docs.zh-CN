---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4d53059ed639dcbf4aa12b5f398d1994004c254a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499708"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getOneDriveUsageStorage(period='D7')?$format=text/csv"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *siteUsageStorageList = [[NSMutableArray alloc] init];
        siteUsageStorageList = [jsonFinal valueForKey:@"value"];
        MSGraphSiteUsageStorage *siteUsageStorage = [[MSGraphSiteUsageStorage alloc] initWithDictionary:[siteUsageStorageList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```