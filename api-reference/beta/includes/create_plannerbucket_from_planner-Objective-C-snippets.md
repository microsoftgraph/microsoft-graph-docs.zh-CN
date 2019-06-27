---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 95f1f60f7d012d92925b68d669432a8cf11c8ce6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35318314"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/buckets"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPlannerBucket *plannerBucket = [[MSGraphPlannerBucket alloc] init];
[plannerBucket setName:@"Advertising"];
[plannerBucket setPlanId:@"xqQg5FS2LkCp935s-FIFm2QAFkHM"];
[plannerBucket setOrderHint:@" !"];

NSError *error;
NSData *plannerBucketData = [plannerBucket getSerializedDataWithError:&error];
[urlRequest setHTTPBody:plannerBucketData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```