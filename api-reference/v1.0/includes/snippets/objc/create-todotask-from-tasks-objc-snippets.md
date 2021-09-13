---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 152aa3d4d3907c7617ee4798b4546e9b350ca0806985e738b78b9350699e6591
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104270"
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