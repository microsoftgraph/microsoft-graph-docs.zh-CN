---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e95a63fec5c568a7fdab1b2b6c094d19ade4300f
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573187"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/tasks/{id}/progressTaskBoardFormat"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"return=representation" forHTTPHeaderField:@"Prefer"];
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