---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5341e5967f51483ab7205ea84bd1507d6b8a1c7d
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920357"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/apiConnectors"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityApiConnector *identityApiConnector = [[MSGraphIdentityApiConnector alloc] init];
[identityApiConnector setDisplayName:@"Test API"];
[identityApiConnector setTargetUrl:@"https://someotherapi.com/api"];
MSGraphApiAuthenticationConfigurationBase *authenticationConfiguration = [[MSGraphApiAuthenticationConfigurationBase alloc] init];
[authenticationConfiguration setPkcs12Value:@"eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA"];
[authenticationConfiguration setPassword:@"CertificatePassword"];
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