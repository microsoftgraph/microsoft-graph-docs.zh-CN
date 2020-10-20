---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09c2d1613aa4c64e7534819b883ea72c8d8e88bd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620598"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/tasks/AAMkADA1MTHgwAAA="]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"outlook.timezone=\"Eastern Standard Time\"" forHTTPHeaderField:@"Prefer"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOutlookTask *outlookTask = [[MSGraphOutlookTask alloc] init];
MSGraphDateTimeTimeZone *dueDateTime = [[MSGraphDateTimeTimeZone alloc] init];
[dueDateTime setDateTime: "2016-05-06T16:00:00"];
[dueDateTime setTimeZone:@"Eastern Standard Time"];
[outlookTask setDueDateTime:dueDateTime];

NSError *error;
NSData *outlookTaskData = [outlookTask getSerializedDataWithError:&error];
[urlRequest setHTTPBody:outlookTaskData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```