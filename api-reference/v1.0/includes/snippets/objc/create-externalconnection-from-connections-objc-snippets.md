---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03c2adf356d2c8f476b7bb61e452efc82d0ec233
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580114"
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