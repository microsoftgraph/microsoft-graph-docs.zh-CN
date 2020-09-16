---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2b1f7f663f4250acd6595536bf1447eec30a8ed
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843081"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTodoTask *todoTask = [[MSGraphTodoTask alloc] init];
MSGraphDateTimeTimeZone *dueDateTime = [[MSGraphDateTimeTimeZone alloc] init];
[dueDateTime setDateTime: "2020-07-25T16:00:00"];
[dueDateTime setTimeZone:@"Eastern Standard Time"];
[todoTask setDueDateTime:dueDateTime];

NSError *error;
NSData *todoTaskData = [todoTask getSerializedDataWithError:&error];
[urlRequest setHTTPBody:todoTaskData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```