---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86bd2654dda90c2ca13872347cd4b66e3b884926
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462462"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/termStore/sets/{setId}/terms/{termId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTermStoreTerm *term = [[MSGraphTermStoreTerm alloc] init];
NSMutableArray *labelsList = [[NSMutableArray alloc] init];
MSGraphTermStoreLocalizedLabel *labels = [[MSGraphTermStoreLocalizedLabel alloc] init];
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