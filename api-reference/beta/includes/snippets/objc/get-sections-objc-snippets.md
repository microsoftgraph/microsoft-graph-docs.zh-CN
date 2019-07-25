---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 611d1d47320484eebae4aee29cac7643b1324147
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895391"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onenote/sectionGroups/{id}/sections"]]];
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