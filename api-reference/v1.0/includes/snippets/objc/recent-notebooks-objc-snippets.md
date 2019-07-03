---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 90cc7a433f5b42cb70a0093880287f778c147048
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463032"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *recentNotebookList = [[NSMutableArray alloc] init];
        recentNotebookList = [jsonFinal valueForKey:@"value"];
        MSGraphRecentNotebook *recentNotebook = [[MSGraphRecentNotebook alloc] initWithDictionary:[recentNotebookList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```