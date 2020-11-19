---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: bb1c4eb21e273def15eeb5cba2381865aaa70442
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214329"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/654b34e7-b48f-4772-a2d4-08f1d0dd014c"]]];
[urlRequest setHTTPMethod:@"PATCH"];

MSGraphAccessReviewInstanceDecisionItem *accessReviewInstanceDecisionItem = [[MSGraphAccessReviewInstanceDecisionItem alloc] init];
[accessReviewInstanceDecisionItem setDecision:@"Approve"];
[accessReviewInstanceDecisionItem setJustification:@"I trust this person"];

NSError *error;
NSData *accessReviewInstanceDecisionItemData = [accessReviewInstanceDecisionItem getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessReviewInstanceDecisionItemData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```