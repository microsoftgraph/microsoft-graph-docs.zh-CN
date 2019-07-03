---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 654906553d9eb9c9487bcea4a001554d4b2c20a8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479022"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/programControlTypes"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *programControlTypeList = [[NSMutableArray alloc] init];
        programControlTypeList = [jsonFinal valueForKey:@"value"];
        MSGraphProgramControlType *programControlType = [[MSGraphProgramControlType alloc] initWithDictionary:[programControlTypeList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```