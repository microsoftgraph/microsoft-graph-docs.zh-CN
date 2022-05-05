---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64c909ef1d0796ea46de08c0c4fc4afa3d7f4f10
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202367"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/domains/contoso.com/federationConfiguration"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphInternalDomainFederation *internalDomainFederation = [[MSGraphInternalDomainFederation alloc] init];
[internalDomainFederation setDisplayName:@"Contoso"];
[internalDomainFederation setIssuerUri:@"http://contoso.com/adfs/services/trust"];
[internalDomainFederation setMetadataExchangeUri:@"https://sts.contoso.com/adfs/services/trust/mex"];
[internalDomainFederation setSigningCertificate:@"MIIE3jCCAsagAwIBAgIQQcyDaZz3MI"];
[internalDomainFederation setPassiveSignInUri:@"https://sts.contoso.com/adfs/ls"];
[internalDomainFederation setPreferredAuthenticationProtocol: [MSGraphAuthenticationProtocol wsFed]];
[internalDomainFederation setActiveSignInUri:@"https://sts.contoso.com/adfs/services/trust/2005/usernamemixed"];
[internalDomainFederation setSignOutUri:@"https://sts.contoso.com/adfs/ls"];
[internalDomainFederation setPromptLoginBehavior: [MSGraphPromptLoginBehavior nativeSupport]];
[internalDomainFederation setIsSignedAuthenticationRequestRequired: true];
[internalDomainFederation setNextSigningCertificate:@"MIIE3jCCAsagAwIBAgIQQcyDaZz3MI"];
[internalDomainFederation setFederatedIdpMfaBehavior: [MSGraphFederatedIdpMfaBehavior rejectMfaByFederatedIdp]];

NSError *error;
NSData *internalDomainFederationData = [internalDomainFederation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:internalDomainFederationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```