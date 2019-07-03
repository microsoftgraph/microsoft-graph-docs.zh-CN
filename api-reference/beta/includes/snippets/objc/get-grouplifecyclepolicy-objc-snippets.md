---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0ff4a26147cdb647e552bf43bfac102ef36b35da
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499954"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groupLifecyclePolicies"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *groupLifecyclePolicyList = [[NSMutableArray alloc] init];
        groupLifecyclePolicyList = [jsonFinal valueForKey:@"value"];
        MSGraphGroupLifecyclePolicy *groupLifecyclePolicy = [[MSGraphGroupLifecyclePolicy alloc] initWithDictionary:[groupLifecyclePolicyList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```