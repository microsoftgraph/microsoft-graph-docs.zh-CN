---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c96ca101f32316ef95573f854ce6da83ceb9117c
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62855756"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/stages/9458f255-dff2-4d86-9a05-69438f49d7f8/decisions/e6cafba0-cbf0-4748-8868-0810c7f4cc06"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessReviewInstanceDecisionItem *accessReviewInstanceDecisionItem = [[MSGraphAccessReviewInstanceDecisionItem alloc] init];
[accessReviewInstanceDecisionItem setDecision:@"Approve"];
[accessReviewInstanceDecisionItem setJustification:@"This person is still on my team"];

NSError *error;
NSData *accessReviewInstanceDecisionItemData = [accessReviewInstanceDecisionItem getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessReviewInstanceDecisionItemData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```