---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e9e3354d65fccaf8fa3eefdb9439d97f589ac903187630ad32e15674eb56b6b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103821"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/termStore/sets/{setId}/terms"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTermStoreTerm *term = [[MSGraphTermStoreTerm alloc] init];
NSMutableArray *labelsList = [[NSMutableArray alloc] init];
MSGraphTermStoreLocalizedLabel *labels = [[MSGraphTermStoreLocalizedLabel alloc] init];
[labels setLanguageTag:@"en-US"];
[labels setName:@"Car"];
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