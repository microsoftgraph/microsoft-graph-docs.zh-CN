---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5de36e8a6505ae664bba8df69a01217f7af02009ef223a45b557b7baffd3cc3b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274191"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/continuousAccessEvaluationPolicy"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphContinuousAccessEvaluationPolicy *continuousAccessEvaluationPolicy = [[MSGraphContinuousAccessEvaluationPolicy alloc] init];
NSMutableArray *usersList = [[NSMutableArray alloc] init];
[usersList addObject: @"88139f01-1f8d-4c06-ad74-a2544cee9aee"];
[continuousAccessEvaluationPolicy setUsers:usersList];
NSMutableArray *groupsList = [[NSMutableArray alloc] init];
[groupsList addObject: @"9972fb3f-7a40-49f5-85f6-129d9dfbd47a"];
[groupsList addObject: @"ea178055-4713-4d9a-a06c-ff17466b7e77"];
[continuousAccessEvaluationPolicy setGroups:groupsList];

NSError *error;
NSData *continuousAccessEvaluationPolicyData = [continuousAccessEvaluationPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:continuousAccessEvaluationPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```