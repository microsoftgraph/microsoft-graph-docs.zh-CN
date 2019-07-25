---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3ba096237aa9429d21068cc33c286bfb6cb7a6d3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710456"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/agreements/'id'"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAgreement *agreement = [[MSGraphAgreement alloc] init];
[agreement setDisplayName:@"displayName-value"];
[agreement setIsViewingBeforeAcceptanceRequired: true];

NSError *error;
NSData *agreementData = [agreement getSerializedDataWithError:&error];
[urlRequest setHTTPBody:agreementData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```