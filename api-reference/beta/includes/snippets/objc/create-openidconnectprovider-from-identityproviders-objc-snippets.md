---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a2377fb2735da0bef8f8abc4db75afeeb444fe5
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566710"
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