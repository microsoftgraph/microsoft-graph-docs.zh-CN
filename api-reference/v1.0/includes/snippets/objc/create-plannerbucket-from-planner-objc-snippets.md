---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd1fec4233d60ef3dbb4a6280d2f2e019c760063
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "35731533"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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