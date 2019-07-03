---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 54642202fa7d87cca46ecc965d665093208b24b1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467502"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/plans/{plan-id}/buckets"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *plannerBucketList = [[NSMutableArray alloc] init];
        plannerBucketList = [jsonFinal valueForKey:@"value"];
        MSGraphPlannerBucket *plannerBucket = [[MSGraphPlannerBucket alloc] initWithDictionary:[plannerBucketList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```