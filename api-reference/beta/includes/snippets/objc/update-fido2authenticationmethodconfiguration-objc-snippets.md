---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54f45d2638162e1593e1b7a6a883f9073e517aa0f1d985f27369f30d7a078543
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163428"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAuthenticationMethodConfiguration *authenticationMethodConfiguration = [[MSGraphAuthenticationMethodConfiguration alloc] init];
[authenticationMethodConfiguration setState: [MSGraphAuthenticationMethodState enabled]];
[authenticationMethodConfiguration setIsAttestationEnforced:@"true"];

NSError *error;
NSData *authenticationMethodConfigurationData = [authenticationMethodConfiguration getSerializedDataWithError:&error];
[urlRequest setHTTPBody:authenticationMethodConfigurationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```