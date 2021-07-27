---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbaaf5000b509f8230fecaad5b73a7969f1380c1
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579952"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/connections/contosohr"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalConnectorsExternalConnection *externalConnection = [[MSGraphExternalConnectorsExternalConnection alloc] init];
[externalConnection setName:@"Contoso HR Service Tickets"];
[externalConnection setDescription:@"Connection to index HR service tickets"];

NSError *error;
NSData *externalConnectionData = [externalConnection getSerializedDataWithError:&error];
[urlRequest setHTTPBody:externalConnectionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```