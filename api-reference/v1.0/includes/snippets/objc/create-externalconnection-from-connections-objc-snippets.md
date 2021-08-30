---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17f74e8b53341f0b6441802092e58a9fdb5e23f212883cd96f2d710a8bc38b27
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278228"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/external/connections"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalConnectorsExternalConnection *externalConnection = [[MSGraphExternalConnectorsExternalConnection alloc] init];
[externalConnection setId:@"contosohr"];
[externalConnection setName:@"Contoso HR"];
[externalConnection setDescription:@"Connection to index Contoso HR system"];

NSError *error;
NSData *externalConnectionData = [externalConnection getSerializedDataWithError:&error];
[urlRequest setHTTPBody:externalConnectionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```