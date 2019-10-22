---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a9f2022a20be97c6807dccc87b9e1888afbe982
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "35723012"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/plans"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPlannerPlan *plannerPlan = [[MSGraphPlannerPlan alloc] init];
[plannerPlan setOwner:@"ebf3b108-5234-4e22-b93d-656d7dae5874"];
[plannerPlan setTitle:@"title-value"];

NSError *error;
NSData *plannerPlanData = [plannerPlan getSerializedDataWithError:&error];
[urlRequest setHTTPBody:plannerPlanData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```