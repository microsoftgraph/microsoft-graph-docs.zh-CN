---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b06f5201b36282d5602c42bb3459ace76504a639
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "35720634"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat"]]];
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