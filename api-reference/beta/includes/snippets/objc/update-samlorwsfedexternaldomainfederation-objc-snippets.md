---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b685ccafe9cfb7c4262741e3d96e24e52d7f6085
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508639"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation/d5a56845-6845-d5a5-4568-a5d54568a5d5"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSamlOrWsFedExternalDomainFederation *samlOrWsFedExternalDomainFederation = [[MSGraphSamlOrWsFedExternalDomainFederation alloc] init];
[samlOrWsFedExternalDomainFederation setDisplayName:@"Contoso name change"];
[samlOrWsFedExternalDomainFederation setIssuerUri:@"http://contoso-test.com/adfs/services/trust"];
[samlOrWsFedExternalDomainFederation setMetadataExchangeUri: null];
[samlOrWsFedExternalDomainFederation setSigningCertificate:@"M66C6DCCAdCgAwIBAgIQQ6vYJIVKQ"];
[samlOrWsFedExternalDomainFederation setPassiveSignInUri:@"https://contoso-test.com/adfs/ls/"];
[samlOrWsFedExternalDomainFederation setPreferredAuthenticationProtocol: [MSGraphAuthenticationProtocol wsFed]];

NSError *error;
NSData *samlOrWsFedExternalDomainFederationData = [samlOrWsFedExternalDomainFederation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:samlOrWsFedExternalDomainFederationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```