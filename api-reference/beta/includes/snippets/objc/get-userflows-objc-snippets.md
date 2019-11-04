---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cc8d8224a32fc58726b1daf03a56e6f04bfacd7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938587"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/userFlows"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *identityUserFlowList = [[NSMutableArray alloc] init];
        identityUserFlowList = [jsonFinal valueForKey:@"value"];
        MSGraphIdentityUserFlow *identityUserFlow = [[MSGraphIdentityUserFlow alloc] initWithDictionary:[identityUserFlowList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```