---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00364a979db4b0bbc8964e9c9bd3cb63481745ac
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240636"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/accessReviews/policy"]]];
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