---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab2c5abc0ebec4d7fbdb3c68b117e114d7f122f4
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610154"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/taskGroups"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOutlookTaskGroup *outlookTaskGroup = [[MSGraphOutlookTaskGroup alloc] init];
[outlookTaskGroup setName:@"Leisure tasks"];

NSError *error;
NSData *outlookTaskGroupData = [outlookTaskGroup getSerializedDataWithError:&error];
[urlRequest setHTTPBody:outlookTaskGroupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```