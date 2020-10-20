---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65bc454004be7a84b0bc88d0a92bb376a9954e41
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603576"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/outlook/tasks/AAMkADA1MHgwAAA="]]];
[urlRequest setHTTPMethod:@"GET"];
[urlRequest setValue:@"outlook.timezone=\"Pacific Standard Time\"" forHTTPHeaderField:@"Prefer"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphOutlookTask *outlookTask = [[MSGraphOutlookTask alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```