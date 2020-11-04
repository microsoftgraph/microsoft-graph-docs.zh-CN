---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d60ee0b76291991de4dce2f11271675c94cce272
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904432"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/todo/lists/AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM/tasks"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTodoTask *todoTask = [[MSGraphTodoTask alloc] init];
[todoTask setTitle:@"A new task"];
NSMutableArray *linkedResourcesList = [[NSMutableArray alloc] init];
MSGraphLinkedResource *linkedResources = [[MSGraphLinkedResource alloc] init];
[linkedResources setWebUrl:@"http://microsoft.com"];
[linkedResources setApplicationName:@"Microsoft"];
[linkedResources setDisplayName:@"Microsoft"];
[linkedResourcesList addObject: linkedResources];
[todoTask setLinkedResources:linkedResourcesList];

NSError *error;
NSData *todoTaskData = [todoTask getSerializedDataWithError:&error];
[urlRequest setHTTPBody:todoTaskData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```