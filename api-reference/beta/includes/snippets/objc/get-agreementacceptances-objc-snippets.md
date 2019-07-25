---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 706c9e37b113440f3070abc57890f0a62939e0f7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716580"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/agreementAcceptances"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *agreementAcceptanceList = [[NSMutableArray alloc] init];
        agreementAcceptanceList = [jsonFinal valueForKey:@"value"];
        MSGraphAgreementAcceptance *agreementAcceptance = [[MSGraphAgreementAcceptance alloc] initWithDictionary:[agreementAcceptanceList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```