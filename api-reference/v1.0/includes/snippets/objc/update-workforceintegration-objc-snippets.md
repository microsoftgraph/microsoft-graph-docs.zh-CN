---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23c6985140dd44628a4e1e853bd6c98986ca68f00d7911daf84e808a19f5de35
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161959"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teamwork/workforceIntegrations/{workforceIntegrationId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
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
[workforceIntegration setSupportedEntities: [MSGraphWorkforceIntegrationSupportedEntities none]];

NSError *error;
NSData *workforceIntegrationData = [workforceIntegration getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workforceIntegrationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```