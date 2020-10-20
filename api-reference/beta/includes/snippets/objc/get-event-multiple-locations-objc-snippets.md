---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f8ba4a2d2e4bda99b843d70981ec002689d7351
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620330"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/events/AAMkADAGAADDdm4NAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphEvent *event = [[MSGraphEvent alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```