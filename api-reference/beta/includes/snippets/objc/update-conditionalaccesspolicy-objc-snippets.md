---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a32e47b2a3146cc83a4531b93045be180f16c7a1
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936709"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/conditionalAccess/policies/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphConditionalAccessPolicy *conditionalAccessPolicy = [[MSGraphConditionalAccessPolicy alloc] init];
MSGraphConditionalAccessConditionSet *conditions = [[MSGraphConditionalAccessConditionSet alloc] init];
NSMutableArray *signInRiskLevelsList = [[NSMutableArray alloc] init];
[signInRiskLevelsList addObject: @"high"];
[signInRiskLevelsList addObject: @"medium"];
[signInRiskLevelsList addObject: @"low"];
[conditions setSignInRiskLevels:signInRiskLevelsList];
[conditionalAccessPolicy setConditions:conditions];

NSError *error;
NSData *conditionalAccessPolicyData = [conditionalAccessPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:conditionalAccessPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```