---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce54119526e53467940717622174fc39b21775aac98a2328af50b791b9f02f64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902742"
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