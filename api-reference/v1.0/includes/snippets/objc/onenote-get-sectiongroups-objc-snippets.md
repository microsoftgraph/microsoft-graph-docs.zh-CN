---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7838c83dec3ec28254a888c7ed79ae3566201a15
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855121"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onenote/sectionGroups"]]];
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