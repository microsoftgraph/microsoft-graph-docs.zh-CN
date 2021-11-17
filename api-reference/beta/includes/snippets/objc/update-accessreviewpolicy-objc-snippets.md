---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f49a4647a5c27e19e01103a6fe9cc0c02dd3c08913cb5e9d1e101e344063798
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902638"
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