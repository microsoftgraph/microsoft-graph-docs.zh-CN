---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 88cf0d89d0c11421e321ea7c711e904ac4440cd1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35322936"
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