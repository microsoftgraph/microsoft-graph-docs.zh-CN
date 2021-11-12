---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 263c82a9e71f605e3919d46d2272f567c13a8c1f1313cec1972c0cad4888ef2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273979"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onenote/notebooks/{id}/sections"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOnenoteSection *onenoteSection = [[MSGraphOnenoteSection alloc] init];
[onenoteSection setDisplayName:@"Section name"];

NSError *error;
NSData *onenoteSectionData = [onenoteSection getSerializedDataWithError:&error];
[urlRequest setHTTPBody:onenoteSectionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```