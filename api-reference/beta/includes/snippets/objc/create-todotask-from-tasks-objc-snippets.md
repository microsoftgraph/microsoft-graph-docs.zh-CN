---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9845c93bd945ca30481ae19643dd62fa1b7d1ed40ba55ed5a6c65ac9d7b34352
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903633"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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