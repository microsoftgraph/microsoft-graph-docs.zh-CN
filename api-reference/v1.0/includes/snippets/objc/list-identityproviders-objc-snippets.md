---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c987f3f17b03692cc330c8526c0cfd6feb80e153
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509290"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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