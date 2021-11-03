---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abb5c21917bce79c081839094de1f13aa0872365
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60718047"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/continuousAccessEvaluationPolicy"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphContinuousAccessEvaluationPolicy *continuousAccessEvaluationPolicy = [[MSGraphContinuousAccessEvaluationPolicy alloc] init];
[continuousAccessEvaluationPolicy setMigrate: true];

NSError *error;
NSData *continuousAccessEvaluationPolicyData = [continuousAccessEvaluationPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:continuousAccessEvaluationPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```