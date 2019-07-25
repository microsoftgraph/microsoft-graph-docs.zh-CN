---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ba698f4f2e8db19ebcd766921f0a87624c18b379
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717525"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites?search=%7Bquery%7D"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *siteList = [[NSMutableArray alloc] init];
        siteList = [jsonFinal valueForKey:@"value"];
        MSGraphSite *site = [[MSGraphSite alloc] initWithDictionary:[siteList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```