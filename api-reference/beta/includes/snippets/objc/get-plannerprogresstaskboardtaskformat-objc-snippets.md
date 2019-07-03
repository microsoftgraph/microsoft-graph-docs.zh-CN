---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c4c815efc630d73938e014ffd7ddd90a6f554fbe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499872"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/tasks/'id'/progressTaskBoardFormat"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphPlannerProgressTaskBoardTaskFormat *plannerProgressTaskBoardTaskFormat = [[MSGraphPlannerProgressTaskBoardTaskFormat alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```