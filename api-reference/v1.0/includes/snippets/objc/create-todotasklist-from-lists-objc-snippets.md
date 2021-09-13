---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0840fb2a35928f15a0a8508d21fba0bc4d559d0f6fac0e45070e2296a66e5ebb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161770"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/todo/lists"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTodoTaskList *todoTaskList = [[MSGraphTodoTaskList alloc] init];
[todoTaskList setDisplayName:@"Travel items"];

NSError *error;
NSData *todoTaskListData = [todoTaskList getSerializedDataWithError:&error];
[urlRequest setHTTPBody:todoTaskListData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```