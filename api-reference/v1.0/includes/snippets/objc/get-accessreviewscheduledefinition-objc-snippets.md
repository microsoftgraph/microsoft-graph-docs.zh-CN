---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32bd7500c2a56f96ab809d2e387f6acec371acca3016dd5fd1f52fbfeb13ad00
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332450"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/accessReviews/definitions/3856fd6f-36e2-4152-97c9-76070d19f730"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphAccessReviewScheduleDefinition *accessReviewScheduleDefinition = [[MSGraphAccessReviewScheduleDefinition alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```