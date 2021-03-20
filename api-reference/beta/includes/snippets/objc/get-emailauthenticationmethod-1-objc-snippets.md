---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a07275f4dea9595b99108b0aac1c236cbe43f58
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950966"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphEmailAuthenticationMethod *emailAuthenticationMethod = [[MSGraphEmailAuthenticationMethod alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```