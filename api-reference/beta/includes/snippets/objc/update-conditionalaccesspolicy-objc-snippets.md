---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64fd03bdffaab07c9270328ed85648f750a478c00042124296acfd925bf7b8e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105236"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/conditionalAccess/policies/{id}"]]];
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