---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 265d7c5d526d9f987b97cdd00b1a2b3154a643aff044c920feb43f0161758e82
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218910"
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