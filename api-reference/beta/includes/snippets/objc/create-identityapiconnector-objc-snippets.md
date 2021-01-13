---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1e1727525b431367d2027642e7f1813ddc5b955
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844539"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/apiConnectors"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityApiConnector *identityApiConnector = [[MSGraphIdentityApiConnector alloc] init];
[identityApiConnector setDisplayName:@"Test API"];
[identityApiConnector setTargetUrl:@"https://someapi.com/api"];
MSGraphApiAuthenticationConfigurationBase *authenticationConfiguration = [[MSGraphApiAuthenticationConfigurationBase alloc] init];
[authenticationConfiguration setUsername:@"<USERNAME>"];
[authenticationConfiguration setPassword:@"<PASSWORD>"];
[identityApiConnector setAuthenticationConfiguration:authenticationConfiguration];

NSError *error;
NSData *identityApiConnectorData = [identityApiConnector getSerializedDataWithError:&error];
[urlRequest setHTTPBody:identityApiConnectorData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```