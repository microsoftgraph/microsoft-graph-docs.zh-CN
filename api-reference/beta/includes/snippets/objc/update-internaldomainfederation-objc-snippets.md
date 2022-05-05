---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07a528e297a276c197e81ea27a792dfe6ccd94b8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211730"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/domains/contoso.com/federationConfiguration/6601d14b-d113-8f64-fda2-9b5ddda18ecc"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphInternalDomainFederation *internalDomainFederation = [[MSGraphInternalDomainFederation alloc] init];
[internalDomainFederation setDisplayName:@"Contoso name change"];
[internalDomainFederation setFederatedIdpMfaBehavior: [MSGraphFederatedIdpMfaBehavior acceptIfMfaDoneByFederatedIdp]];

NSError *error;
NSData *internalDomainFederationData = [internalDomainFederation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:internalDomainFederationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```