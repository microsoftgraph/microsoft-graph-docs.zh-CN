---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f7453e5d42593f0dd3d90d3ea26427845ac11333558420d10353d5c707d406b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104118"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphAccessReviewScheduleDefinition *accessReviewScheduleDefinition = [[MSGraphAccessReviewScheduleDefinition alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```