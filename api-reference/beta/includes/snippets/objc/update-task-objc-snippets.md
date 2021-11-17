---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e86835d29e411802ffdb7ae87938e3ba89809aac2348257fa237a78e73f39ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279596"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c/tasks/d036638b-1272-4bba-9227-732463823ed3"]]];
[urlRequest setHTTPMethod:@"PATCH"];

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