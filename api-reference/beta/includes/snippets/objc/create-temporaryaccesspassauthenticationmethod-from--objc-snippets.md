---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4274ba154ddd30162f7c56e60723771847f361302643ccbb545b4c5e15d6f39
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904006"
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