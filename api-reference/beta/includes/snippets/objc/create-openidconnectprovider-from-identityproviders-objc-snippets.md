---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d28fcc29db84e8a13b7bce5cd559e4ce2587c8bf93532237aac0548f3524beb0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278964"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityProviders"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityProvider *identityProvider = [[MSGraphIdentityProvider alloc] init];
[identityProvider setName:@"Login with the Contoso identity provider"];
[identityProvider setType:@"OpenIDConnect"];
[identityProvider setClientId:@"56433757-cadd-4135-8431-2c9e3fd68ae8"];
[identityProvider setClientSecret:@"12345"];
MSGraphClaimsMapping *claimsMapping = [[MSGraphClaimsMapping alloc] init];
[claimsMapping setUserId:@"myUserId"];
[claimsMapping setGivenName:@"myGivenName"];
[claimsMapping setSurname:@"mySurname"];
[claimsMapping setEmail:@"myEmail"];
[claimsMapping setDisplayName:@"myDisplayName"];
[identityProvider setClaimsMapping:claimsMapping];
[identityProvider setDomainHint:@"mycustomoidc"];
[identityProvider setMetadataUrl:@"https://mycustomoidc.com/.well-known/openid-configuration"];
[identityProvider setResponseMode: [MSGraphOpenIdConnectResponseMode form_post]];
[identityProvider setResponseType: [MSGraphOpenIdConnectResponseTypes code]];
[identityProvider setScope:@"openid"];

NSError *error;
NSData *identityProviderData = [identityProvider getSerializedDataWithError:&error];
[urlRequest setHTTPBody:identityProviderData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```