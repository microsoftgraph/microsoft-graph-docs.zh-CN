---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b75be4ed5156552d46cb5c295d101b3f84d8392
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944621"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUserFlowLanguageConfiguration *userFlowLanguageConfiguration = [[MSGraphUserFlowLanguageConfiguration alloc] init];
[userFlowLanguageConfiguration setId:@"es-ES"];
[userFlowLanguageConfiguration setIsEnabled: true];

NSError *error;
NSData *userFlowLanguageConfigurationData = [userFlowLanguageConfiguration getSerializedDataWithError:&error];
[urlRequest setHTTPBody:userFlowLanguageConfigurationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```