---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 297f31902b8a326f359d8e74df31aad906736e9a7c6917e6f08b9e4f5e1bdfd5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164027"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/todo/lists/AAMkADIyAAAhrbPWAAA="]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTodoTaskList *todoTaskList = [[MSGraphTodoTaskList alloc] init];
[todoTaskList setDisplayName:@"Vacation Plan"];

NSError *error;
NSData *todoTaskListData = [todoTaskList getSerializedDataWithError:&error];
[urlRequest setHTTPBody:todoTaskListData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```