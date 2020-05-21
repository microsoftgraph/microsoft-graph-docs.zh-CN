---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c750e5955c57d314472dde4a469d64d1a632a6d
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333678"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/oauth2PermissionGrants"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOAuth2PermissionGrant *oAuth2PermissionGrant = [[MSGraphOAuth2PermissionGrant alloc] init];
[oAuth2PermissionGrant setClientId:@"clientId-value"];
[oAuth2PermissionGrant setConsentType:@"consentType-value"];
[oAuth2PermissionGrant setPrincipalId:@"principalId-value"];
[oAuth2PermissionGrant setResourceId:@"resourceId-value"];
[oAuth2PermissionGrant setScope:@"scope-value"];
[oAuth2PermissionGrant setStartTime: "2016-10-19T10:37:00Z"];
[oAuth2PermissionGrant setExpiryTime: "2016-10-19T10:37:00Z"];

NSError *error;
NSData *oAuth2PermissionGrantData = [oAuth2PermissionGrant getSerializedDataWithError:&error];
[urlRequest setHTTPBody:oAuth2PermissionGrantData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```