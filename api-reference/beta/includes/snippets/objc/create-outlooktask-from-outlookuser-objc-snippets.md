---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 694731f0faaf0e2061afe48d83e64cec334e0ca6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877305"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/tasks"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"outlook.timezone=\"Pacific Standard Time\"" forHTTPHeaderField:@"Prefer"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOutlookTask *outlookTask = [[MSGraphOutlookTask alloc] init];
[outlookTask setSubject:@"Shop for children's weekend"];
MSGraphDateTimeTimeZone *startDateTime = [[MSGraphDateTimeTimeZone alloc] init];
[startDateTime setDateTime: "2016-05-03T09:00:00"];
[startDateTime setTimeZone:@"Eastern Standard Time"];
[outlookTask setStartDateTime:startDateTime];
MSGraphDateTimeTimeZone *dueDateTime = [[MSGraphDateTimeTimeZone alloc] init];
[dueDateTime setDateTime: "2016-05-05T16:00:00"];
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