---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 670cdbae0bb7bd0175e88ef289af86d2efcad8c6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871199"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/userCredentialUsageDetails"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *userCredentialUsageDetailsList = [[NSMutableArray alloc] init];
        userCredentialUsageDetailsList = [jsonFinal valueForKey:@"value"];
        MSGraphUserCredentialUsageDetails *userCredentialUsageDetails = [[MSGraphUserCredentialUsageDetails alloc] initWithDictionary:[userCredentialUsageDetailsList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```