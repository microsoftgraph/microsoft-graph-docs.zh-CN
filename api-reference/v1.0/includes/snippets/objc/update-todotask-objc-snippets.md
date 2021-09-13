---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d43563f5af1d3b8881534c99d525788e847f5e9562b49cadf5ec08287894d1af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161769"
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