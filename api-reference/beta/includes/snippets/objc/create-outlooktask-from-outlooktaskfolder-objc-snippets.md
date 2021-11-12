---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 243877d2350965fe2a8dbb878708592a3e3f40413abdc7ee6dffb6398481fc3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163393"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/taskfolders('AAMkADIyAAAhrbPXAAA=')/tasks"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOutlookTask *outlookTask = [[MSGraphOutlookTask alloc] init];
[outlookTask setSubject:@"Shop for dinner"];
MSGraphDateTimeTimeZone *startDateTime = [[MSGraphDateTimeTimeZone alloc] init];
[startDateTime setDateTime: "2016-04-23T18:00:00"];
[startDateTime setTimeZone:@"Pacific Standard Time"];
[outlookTask setStartDateTime:startDateTime];
MSGraphDateTimeTimeZone *dueDateTime = [[MSGraphDateTimeTimeZone alloc] init];
[dueDateTime setDateTime: "2016-04-25T13:00:00"];
[dueDateTime setTimeZone:@"Pacific Standard Time"];
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