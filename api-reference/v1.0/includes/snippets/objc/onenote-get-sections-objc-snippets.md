---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9fb1f5bcdd3af5b5c31649899387c2969ac9014d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887973"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onenote/sections"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *onenoteSectionList = [[NSMutableArray alloc] init];
        onenoteSectionList = [jsonFinal valueForKey:@"value"];
        MSGraphOnenoteSection *onenoteSection = [[MSGraphOnenoteSection alloc] initWithDictionary:[onenoteSectionList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```