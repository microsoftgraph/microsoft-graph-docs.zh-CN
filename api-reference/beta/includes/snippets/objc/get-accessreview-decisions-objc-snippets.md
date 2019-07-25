---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 865ff0c77f7200af6b0f522bb57fc5a7e56fc361
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710937"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *accessReviewDecisionList = [[NSMutableArray alloc] init];
        accessReviewDecisionList = [jsonFinal valueForKey:@"value"];
        MSGraphAccessReviewDecision *accessReviewDecision = [[MSGraphAccessReviewDecision alloc] initWithDictionary:[accessReviewDecisionList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```