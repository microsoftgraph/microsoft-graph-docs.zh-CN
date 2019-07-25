---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e391cf1b71fa78bcb64c88da80e5aec83d92654e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720382"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/planner/recentPlans"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *plannerPlanList = [[NSMutableArray alloc] init];
        plannerPlanList = [jsonFinal valueForKey:@"value"];
        MSGraphPlannerPlan *plannerPlan = [[MSGraphPlannerPlan alloc] initWithDictionary:[plannerPlanList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```