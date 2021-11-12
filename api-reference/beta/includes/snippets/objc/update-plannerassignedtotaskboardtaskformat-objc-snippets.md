---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c4e0f5876e6a882a9fda1f0a7bb834f7569cacdd8add2378497e594045ab632
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278919"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat"]]];
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