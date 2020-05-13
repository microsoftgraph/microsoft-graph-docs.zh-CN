---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 301593abc5463fc665b506beed920d1e96d2e186
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "40870451"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teamwork/workforceIntegrations"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkforceIntegration *workforceIntegrations = [[MSGraphWorkforceIntegration alloc] init];
[workforceIntegrations setDisplayName:@"displayName-value"];
[workforceIntegrations setApiVersion: 99];
MSGraphWorkforceIntegrationEncryption *encryption = [[MSGraphWorkforceIntegrationEncryption alloc] init];
[encryption setProtocol: [MSGraphWorkforceIntegrationEncryptionProtocol sharedSecret]];
[encryption setSecret:@"secret-value"];
[workforceIntegrations setEncryption:encryption];
[workforceIntegrations setIsActive: true];
[workforceIntegrations setUrl:@"url-value"];
[workforceIntegrations setSupports: [MSGraphWorkforceIntegrationSupportedEntities none]];

NSError *error;
NSData *workforceIntegrationsData = [workforceIntegrations getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workforceIntegrationsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```