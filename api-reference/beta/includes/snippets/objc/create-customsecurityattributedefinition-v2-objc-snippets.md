---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45baf1da214a17a9eb285d351e02baec37ccfade
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226801"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directory/customSecurityAttributeDefinitions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCustomSecurityAttributeDefinition *customSecurityAttributeDefinition = [[MSGraphCustomSecurityAttributeDefinition alloc] init];
[customSecurityAttributeDefinition setAttributeSet:@"Engineering"];
[customSecurityAttributeDefinition setDescription:@"Active projects for user"];
[customSecurityAttributeDefinition setIsCollection: true];
[customSecurityAttributeDefinition setIsSearchable: true];
[customSecurityAttributeDefinition setName:@"Project"];
[customSecurityAttributeDefinition setStatus:@"Available"];
[customSecurityAttributeDefinition setType:@"String"];
[customSecurityAttributeDefinition setUsePreDefinedValuesOnly: true];

NSError *error;
NSData *customSecurityAttributeDefinitionData = [customSecurityAttributeDefinition getSerializedDataWithError:&error];
[urlRequest setHTTPBody:customSecurityAttributeDefinitionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```