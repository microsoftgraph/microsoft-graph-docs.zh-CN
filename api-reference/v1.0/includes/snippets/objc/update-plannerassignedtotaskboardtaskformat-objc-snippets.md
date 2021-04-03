---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 808e0a0041bd56cd0b5b97c7a9f3fb0c800ef89c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573141"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/tasks/{task-id}/assignedToTaskBoardFormat"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"return=representation" forHTTPHeaderField:@"Prefer"];
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