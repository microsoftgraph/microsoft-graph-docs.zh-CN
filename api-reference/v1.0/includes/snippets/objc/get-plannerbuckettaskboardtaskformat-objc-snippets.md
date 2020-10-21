---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88cf0d89d0c11421e321ea7c711e904ac4440cd1
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605959"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/tasks/{task-id}/bucketTaskBoardFormat"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphPlannerBucketTaskBoardTaskFormat *plannerBucketTaskBoardTaskFormat = [[MSGraphPlannerBucketTaskBoardTaskFormat alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```