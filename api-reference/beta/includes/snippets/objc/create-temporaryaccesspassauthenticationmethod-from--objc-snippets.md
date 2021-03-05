---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 727f825adbfda4a7fae8582c8d9646cf6a72b3bd
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475070"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/kim@contoso.com/authentication/temporaryAccessPassMethods"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTemporaryAccessPassAuthenticationMethod *temporaryAccessPassAuthenticationMethod = [[MSGraphTemporaryAccessPassAuthenticationMethod alloc] init];
[temporaryAccessPassAuthenticationMethod setStartDateTime: "2021-01-26T00:00:00Z"];
[temporaryAccessPassAuthenticationMethod setLifetimeInMinutes: 60];
[temporaryAccessPassAuthenticationMethod setIsUsableOnce: false];

NSError *error;
NSData *temporaryAccessPassAuthenticationMethodData = [temporaryAccessPassAuthenticationMethod getSerializedDataWithError:&error];
[urlRequest setHTTPBody:temporaryAccessPassAuthenticationMethodData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```