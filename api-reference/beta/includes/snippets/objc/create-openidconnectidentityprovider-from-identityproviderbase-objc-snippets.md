---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f0fbbdbdbaa902fef68afb1b4358af9fe497275381fda70ac0bdf303d0996c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162080"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/identityProviders"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityProviderBase *identityProviderBase = [[MSGraphIdentityProviderBase alloc] init];
[identityProviderBase setDisplayName:@"Login with the Contoso identity provider"];
[identityProviderBase setClientId:@"56433757-cadd-4135-8431-2c9e3fd68ae8"];
[identityProviderBase setClientSecret:@"12345"];
MSGraphClaimsMapping *claimsMapping = [[MSGraphClaimsMapping alloc] init];
[claimsMapping setUserId:@"myUserId"];
[claimsMapping setGivenName:@"myGivenName"];
[claimsMapping setSurname:@"mySurname"];
[claimsMapping setEmail:@"myEmail"];
[claimsMapping setDisplayName:@"myDisplayName"];
[identityProviderBase setClaimsMapping:claimsMapping];
[identityProviderBase setDomainHint:@"mycustomoidc"];
[identityProviderBase setMetadataUrl:@"https://mycustomoidc.com/.well-known/openid-configuration"];
[identityProviderBase setResponseMode: [MSGraphOpenIdConnectResponseMode form_post]];
[identityProviderBase setResponseType: [MSGraphOpenIdConnectResponseTypes code]];
[identityProviderBase setScope:@"openid"];

NSError *error;
NSData *identityProviderBaseData = [identityProviderBase getSerializedDataWithError:&error];
[urlRequest setHTTPBody:identityProviderBaseData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```