---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a0045dfcf4f1d66579f09d0d8e10e8ccc9d028e2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858340"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/{id}/owners"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *directoryObjectList = [[NSMutableArray alloc] init];
        directoryObjectList = [jsonFinal valueForKey:@"value"];
        MSGraphDirectoryObject *directoryObject = [[MSGraphDirectoryObject alloc] initWithDictionary:[directoryObjectList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```