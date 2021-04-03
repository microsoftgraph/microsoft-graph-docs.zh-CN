---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5a8c1ec048b4ffa51592e6091323c279a5528f2
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573191"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"return=representation" forHTTPHeaderField:@"Prefer"];
[urlRequest setValue:@"W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"" forHTTPHeaderField:@"If-Match"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPlannerPlanDetails *plannerPlanDetails = [[MSGraphPlannerPlanDetails alloc] init];
MSGraphPlannerUserIds *sharedWith = [[MSGraphPlannerUserIds alloc] init];
[sharedWith set6463a5ce-2119-4198-9f2a-628761df4a62: true];
[sharedWith setD95e6152-f683-4d78-9ff5-67ad180fea4a: false];
[plannerPlanDetails setSharedWith:sharedWith];
MSGraphPlannerCategoryDescriptions *categoryDescriptions = [[MSGraphPlannerCategoryDescriptions alloc] init];
[categoryDescriptions setCategory1:@"Indoors"];
[categoryDescriptions setCategory3: null];
[plannerPlanDetails setCategoryDescriptions:categoryDescriptions];

NSError *error;
NSData *plannerPlanDetailsData = [plannerPlanDetails getSerializedDataWithError:&error];
[urlRequest setHTTPBody:plannerPlanDetailsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```