---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23bc95ff02c4170d4730a804b2f020385bfd1b37
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844343"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/apiConnectors/{identityApiConnectorId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityApiConnector *identityApiConnector = [[MSGraphIdentityApiConnector alloc] init];
[identityApiConnector setDisplayName:@"New Test API"];
[identityApiConnector setTargetUrl:@"https://otherapi.com/api/endpoint"];
MSGraphApiAuthenticationConfigurationBase *authenticationConfiguration = [[MSGraphApiAuthenticationConfigurationBase alloc] init];
[authenticationConfiguration setUsername:@"<NEW_USERNAME>"];
[authenticationConfiguration setPassword:@"<NEW_PASSWORD>"];
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