---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4446a749b6f209a47b7c3e9cb2397826ade311fe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479595"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/oAuth2Permissiongrants"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *oAuth2PermissionGrantList = [[NSMutableArray alloc] init];
        oAuth2PermissionGrantList = [jsonFinal valueForKey:@"value"];
        MSGraphOAuth2PermissionGrant *oAuth2PermissionGrant = [[MSGraphOAuth2PermissionGrant alloc] initWithDictionary:[oAuth2PermissionGrantList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```