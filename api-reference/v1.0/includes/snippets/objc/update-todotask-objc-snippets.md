---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a0559ed40a3eb50e080ac337c3c095aba1f9599
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905352"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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