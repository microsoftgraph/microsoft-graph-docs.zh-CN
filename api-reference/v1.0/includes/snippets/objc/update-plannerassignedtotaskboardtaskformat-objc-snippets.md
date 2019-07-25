---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 25ffb31b4ace47f061e7070050f29844d703d0c9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705129"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/tasks/{task-id}/assignedToTaskBoardFormat"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"" forHTTPHeaderField:@"If-Match"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPlannerAssignedToTaskBoardTaskFormat *plannerAssignedToTaskBoardTaskFormat = [[MSGraphPlannerAssignedToTaskBoardTaskFormat alloc] init];
MSGraphPlannerOrderHintsByAssignee *orderHintsByAssignee = [[MSGraphPlannerOrderHintsByAssignee alloc] init];
[orderHintsByAssignee setAaa27244-1db4-476a-a5cb-004607466324:@"8566473P 957764Jk!"];
[plannerAssignedToTaskBoardTaskFormat setOrderHintsByAssignee:orderHintsByAssignee];

NSError *error;
NSData *plannerAssignedToTaskBoardTaskFormatData = [plannerAssignedToTaskBoardTaskFormat getSerializedDataWithError:&error];
[urlRequest setHTTPBody:plannerAssignedToTaskBoardTaskFormatData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```