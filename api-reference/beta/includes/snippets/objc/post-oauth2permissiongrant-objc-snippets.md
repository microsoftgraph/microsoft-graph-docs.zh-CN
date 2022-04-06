---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7ac55d992f7a857fd2589fc37c93e41fcadcc73
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759214"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/oauth2PermissionGrants"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOAuth2PermissionGrant *oAuth2PermissionGrant = [[MSGraphOAuth2PermissionGrant alloc] init];
[oAuth2PermissionGrant setClientId:@"ef969797-201d-4f6b-960c-e9ed5f31dab5"];
[oAuth2PermissionGrant setConsentType:@"AllPrincipals"];
[oAuth2PermissionGrant setResourceId:@"943603e4-e787-4fe9-93d1-e30f749aae39"];
[oAuth2PermissionGrant setScope:@"DelegatedPermissionGrant.ReadWrite.All"];
[oAuth2PermissionGrant setStartTime: "2022-03-17T00:00:00Z"];
[oAuth2PermissionGrant setExpiryTime: "2023-03-17T00:00:00Z"];

NSError *error;
NSData *oAuth2PermissionGrantData = [oAuth2PermissionGrant getSerializedDataWithError:&error];
[urlRequest setHTTPBody:oAuth2PermissionGrantData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```