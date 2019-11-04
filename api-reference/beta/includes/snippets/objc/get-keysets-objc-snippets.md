---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfbd4ed77b57bcdb8d1a514b26dcec53fc264da1
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938333"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/trustFramework/keySets"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *trustFrameworkKeySetList = [[NSMutableArray alloc] init];
        trustFrameworkKeySetList = [jsonFinal valueForKey:@"value"];
        MSGraphTrustFrameworkKeySet *trustFrameworkKeySet = [[MSGraphTrustFrameworkKeySet alloc] initWithDictionary:[trustFrameworkKeySetList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```