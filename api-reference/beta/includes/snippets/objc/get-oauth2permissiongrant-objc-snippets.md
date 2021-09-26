---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80d65a907b5b4c9b53d03ea3f159e19d629ccf8e6d2473408a34e10bd614e356
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164106"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/oauth2PermissionGrants/{id}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphOAuth2PermissionGrant *oAuth2PermissionGrant = [[MSGraphOAuth2PermissionGrant alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```