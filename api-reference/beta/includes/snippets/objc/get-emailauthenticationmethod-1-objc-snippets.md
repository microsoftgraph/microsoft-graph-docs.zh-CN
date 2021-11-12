---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea7c490755653f0cf88e0e19388f8e81eebae29dbf703c3ec0aca2f0b8c5d133
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163233"
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