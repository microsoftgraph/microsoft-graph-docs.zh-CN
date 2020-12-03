---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0143623b7fa99c8e7a494a27648fdddff339fd56
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/02/2020
ms.locfileid: "49556099"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUser *user = [[MSGraphUser alloc] init];
[user setAccountEnabled: true];
[user setDisplayName:@"Adele Vance"];
[user setMailNickname:@"AdeleV"];
[user setUserPrincipalName:@"AdeleV@contoso.onmicrosoft.com"];
MSGraphPasswordProfile *passwordProfile = [[MSGraphPasswordProfile alloc] init];
[passwordProfile setForceChangePasswordNextSignIn: true];
[passwordProfile setPassword:@"xWwvJ]6NMw+bWH-d"];
[user setPasswordProfile:passwordProfile];

NSError *error;
NSData *userData = [user getSerializedDataWithError:&error];
[urlRequest setHTTPBody:userData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```