---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 17c41f2a217f8f66d5d0177c079b2bc828b604aa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728327"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/programs/673a7379-9c38-4f01-bd9d-4fda7260b807/controls"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *programControlList = [[NSMutableArray alloc] init];
        programControlList = [jsonFinal valueForKey:@"value"];
        MSGraphProgramControl *programControl = [[MSGraphProgramControl alloc] initWithDictionary:[programControlList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```