---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62d7ec47bc8953766722566f0c64ff9137197452
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616205"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessReviewReviewer *accessReviewReviewer = [[MSGraphAccessReviewReviewer alloc] init];
[accessReviewReviewer setId:@"006111db-0810-4494-a6df-904d368bd81b"];

NSError *error;
NSData *accessReviewReviewerData = [accessReviewReviewer getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessReviewReviewerData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```