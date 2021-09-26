---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6aba43e6194a02db40c15ca3b84e1896d1449304
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763903"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directory/federationConfigurations/d5a56845-6845-d5a5-4568-a5d54568a5d5/microsoft.graph.samlOrWsFedExternalDomainFederation/domains"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalDomainName *externalDomainName = [[MSGraphExternalDomainName alloc] init];
[externalDomainName setId:@"contososuites.com"];

NSError *error;
NSData *externalDomainNameData = [externalDomainName getSerializedDataWithError:&error];
[urlRequest setHTTPBody:externalDomainNameData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```