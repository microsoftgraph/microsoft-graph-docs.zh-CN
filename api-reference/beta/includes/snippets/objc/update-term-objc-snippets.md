---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09894aaf91452a68e7e9a20bec4156970f4daedd
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330198"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/termStore/sets/{setId}/terms/{termId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTerm *term = [[MSGraphTerm alloc] init];
NSMutableArray *labelsList = [[NSMutableArray alloc] init];
MSGraphLocalizedLabel *labels = [[MSGraphLocalizedLabel alloc] init];
[labels setName:@"changedLabel"];
[labels setLanguageTag:@"en-US"];
[labels setIsDefault: true];
[labelsList addObject: labels];
[term setLabels:labelsList];

NSError *error;
NSData *termData = [term getSerializedDataWithError:&error];
[urlRequest setHTTPBody:termData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```