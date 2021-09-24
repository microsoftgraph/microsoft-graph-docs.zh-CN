---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51dfc1f3ddbf7646a497ebf3c280c7ef83894725
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508485"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directory/federationConfigurations"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityProviderBase *identityProviderBase = [[MSGraphIdentityProviderBase alloc] init];
[identityProviderBase setIssuerUri:@"https://contoso.com/issuerUri"];
[identityProviderBase setDisplayName:@"contoso display name"];
[identityProviderBase setMetadataExchangeUri:@"https://contoso.com/metadataExchangeUri"];
[identityProviderBase setPassiveSignInUri:@"https://contoso.com/signin"];
[identityProviderBase setPreferredAuthenticationProtocol: [MSGraphAuthenticationProtocol wsFed]];
NSMutableArray *domainsList = [[NSMutableArray alloc] init];
MSGraphExternalDomainName *domains = [[MSGraphExternalDomainName alloc] init];
[domains setId:@"contoso.com"];
[domainsList addObject: domains];
[identityProviderBase setDomains:domainsList];
[identityProviderBase setSigningCertificate:@"MIIDADCCAeigAwIBAgIQEX41y8r6"];

NSError *error;
NSData *identityProviderBaseData = [identityProviderBase getSerializedDataWithError:&error];
[urlRequest setHTTPBody:identityProviderBaseData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```