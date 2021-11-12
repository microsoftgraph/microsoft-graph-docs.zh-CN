---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b814e5bdcc928b4f77d8118cca91e88b628858216c85009a12ee20bcb040a83
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163114"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"return=representation" forHTTPHeaderField:@"Prefer"];
[urlRequest setValue:@"W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"" forHTTPHeaderField:@"If-Match"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPlannerBucketTaskBoardTaskFormat *plannerBucketTaskBoardTaskFormat = [[MSGraphPlannerBucketTaskBoardTaskFormat alloc] init];
[plannerBucketTaskBoardTaskFormat setOrderHint:@"A6673H Ejkl!"];

NSError *error;
NSData *plannerBucketTaskBoardTaskFormatData = [plannerBucketTaskBoardTaskFormat getSerializedDataWithError:&error];
[urlRequest setHTTPBody:plannerBucketTaskBoardTaskFormatData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```