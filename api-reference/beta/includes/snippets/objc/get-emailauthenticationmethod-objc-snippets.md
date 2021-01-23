---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a07275f4dea9595b99108b0aac1c236cbe43f58
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945097"
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