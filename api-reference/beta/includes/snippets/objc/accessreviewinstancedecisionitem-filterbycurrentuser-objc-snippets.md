---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e6ace3913ae410eb70008c301f28c594c05a83a2b49543aab4ee12d5a7f2b3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104132"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/accessReviews/definitions/0185aab8-9a7e-44b5-ae36-41b923c3bf87/instances/1234aab8-9a7e-5678-ae36-41b923c3bf87/decisions/filterByCurrentUser(on='reviewer')"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphAccessReviewInstanceDecisionItem *accessReviewInstanceDecisionItem = [[MSGraphAccessReviewInstanceDecisionItem alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```