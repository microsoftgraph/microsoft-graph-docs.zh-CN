---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02391556550aff7435a9286fda24c213097d5813
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994724"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/external/connections"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalConnection *externalConnection = [[MSGraphExternalConnection alloc] init];
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