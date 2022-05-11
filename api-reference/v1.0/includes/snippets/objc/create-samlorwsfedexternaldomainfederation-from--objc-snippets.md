---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51dfc1f3ddbf7646a497ebf3c280c7ef83894725
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315727"
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