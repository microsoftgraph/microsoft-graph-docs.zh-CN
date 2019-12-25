---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f1a1f13eb6dd5182584a7fa4d5dab78011ba3ff
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870573"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teamwork/workforceIntegrations"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkforceIntegration *workforceIntegration = [[MSGraphWorkforceIntegration alloc] init];
[workforceIntegration setDisplayName:@"displayName-value"];
[workforceIntegration setApiVersion: 99];
MSGraphWorkforceIntegrationEncryption *encryption = [[MSGraphWorkforceIntegrationEncryption alloc] init];
[encryption setProtocol: [MSGraphWorkforceIntegrationEncryptionProtocol sharedSecret]];
[encryption setSecret:@"secret-value"];
[workforceIntegration setEncryption:encryption];
[workforceIntegration setIsActive: true];
[workforceIntegration setUrl:@"url-value"];
[workforceIntegration setSupports: [MSGraphWorkforceIntegrationSupportedEntities none]];

NSError *error;
NSData *workforceIntegrationData = [workforceIntegration getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workforceIntegrationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```