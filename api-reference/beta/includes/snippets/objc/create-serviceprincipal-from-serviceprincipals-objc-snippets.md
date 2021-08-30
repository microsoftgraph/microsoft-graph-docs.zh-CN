---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91ce905b17ad2a483da2b4a2cc2288c0dd14a32a10a3448fe6bef18aeb940528
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220776"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphServicePrincipal *servicePrincipal = [[MSGraphServicePrincipal alloc] init];
[servicePrincipal setAppId:@"65415bb1-9267-4313-bbf5-ae259732ee12"];

NSError *error;
NSData *servicePrincipalData = [servicePrincipal getSerializedDataWithError:&error];
[urlRequest setHTTPBody:servicePrincipalData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```