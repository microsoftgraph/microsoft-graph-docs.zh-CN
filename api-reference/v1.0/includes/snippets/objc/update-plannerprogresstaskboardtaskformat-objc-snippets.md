---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c08dda343d3c580f3c6ede7ff14338a103aa3b38
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734774"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/tasks/{task-id}/progressTaskBoardFormat"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"" forHTTPHeaderField:@"If-Match"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPlannerProgressTaskBoardTaskFormat *plannerProgressTaskBoardTaskFormat = [[MSGraphPlannerProgressTaskBoardTaskFormat alloc] init];
[plannerProgressTaskBoardTaskFormat setOrderHint:@"A6673H Ejkl!"];

NSError *error;
NSData *plannerProgressTaskBoardTaskFormatData = [plannerProgressTaskBoardTaskFormat getSerializedDataWithError:&error];
[urlRequest setHTTPBody:plannerProgressTaskBoardTaskFormatData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```