---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bcdec765f996d206b94795c6e5258923006f9904
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480047"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityProviders"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *identityProviderList = [[NSMutableArray alloc] init];
        identityProviderList = [jsonFinal valueForKey:@"value"];
        MSGraphIdentityProvider *identityProvider = [[MSGraphIdentityProvider alloc] initWithDictionary:[identityProviderList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```