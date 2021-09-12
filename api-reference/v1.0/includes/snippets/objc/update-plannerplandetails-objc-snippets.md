---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd5f574c2bf401d3b0ef892e684a24ee86228af5676153a735ce04adb0e7efeb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107002"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/plans/{plan-id}/details"]]];
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