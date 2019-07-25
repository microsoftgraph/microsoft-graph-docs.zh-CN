---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f9a6561e34e24a76f96d4da1c4ba7901a6f4bd78
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874099"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/getCredentialUserRegistrationCount"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *credentialUserRegistrationCountList = [[NSMutableArray alloc] init];
        credentialUserRegistrationCountList = [jsonFinal valueForKey:@"value"];
        MSGraphCredentialUserRegistrationCount *credentialUserRegistrationCount = [[MSGraphCredentialUserRegistrationCount alloc] initWithDictionary:[credentialUserRegistrationCountList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```