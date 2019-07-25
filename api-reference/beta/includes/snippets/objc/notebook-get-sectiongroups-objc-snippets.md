---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9cf18a1e5798a0a7cab31bed9085d1070666218a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879043"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onenote/notebooks/{id}/sectionGroups"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *sectionGroupList = [[NSMutableArray alloc] init];
        sectionGroupList = [jsonFinal valueForKey:@"value"];
        MSGraphSectionGroup *sectionGroup = [[MSGraphSectionGroup alloc] initWithDictionary:[sectionGroupList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```