---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 593af4f75c261033df88a64e0a14d4362d2ea73f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771307"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPrintTask *printTask = [[MSGraphPrintTask alloc] init];
MSGraphPrintTaskStatus *status = [[MSGraphPrintTaskStatus alloc] init];
[status setState: [MSGraphPrintTaskProcessingState completed]];
[status setDescription:@"completed"];
[printTask setStatus:status];

NSError *error;
NSData *printTaskData = [printTask getSerializedDataWithError:&error];
[urlRequest setHTTPBody:printTaskData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```