---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7f7a2b8682941705270a75babd0c6959ccd858c7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478871"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/security/secureScores?$top=1"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *secureScoreList = [[NSMutableArray alloc] init];
        secureScoreList = [jsonFinal valueForKey:@"value"];
        MSGraphSecureScore *secureScore = [[MSGraphSecureScore alloc] initWithDictionary:[secureScoreList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```