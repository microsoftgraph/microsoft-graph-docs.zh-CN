---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ae39165e324a9b0662428739711fb2e63f85a892
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871181"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/credentialUserRegistrationDetails"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *credentialUserRegistrationDetailsList = [[NSMutableArray alloc] init];
        credentialUserRegistrationDetailsList = [jsonFinal valueForKey:@"value"];
        MSGraphCredentialUserRegistrationDetails *credentialUserRegistrationDetails = [[MSGraphCredentialUserRegistrationDetails alloc] initWithDictionary:[credentialUserRegistrationDetailsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```