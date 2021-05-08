---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c767fb1e04f7261340697fdd4b76aa9a197e081b
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240632"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/accessReviewPolicy"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessReviewPolicy *accessReviewPolicy = [[MSGraphAccessReviewPolicy alloc] init];
[accessReviewPolicy setIsGroupOwnerManagementEnabled: true];

NSError *error;
NSData *accessReviewPolicyData = [accessReviewPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessReviewPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```