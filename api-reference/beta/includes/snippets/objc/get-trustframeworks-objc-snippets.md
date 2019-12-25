---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f50427bef362fc01a793b87c54df4f50573035b2
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "35716748"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/trustFramework/policies"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *trustFrameworkPolicyList = [[NSMutableArray alloc] init];
        trustFrameworkPolicyList = [jsonFinal valueForKey:@"value"];
        MSGraphTrustFrameworkPolicy *trustFrameworkPolicy = [[MSGraphTrustFrameworkPolicy alloc] initWithDictionary:[trustFrameworkPolicyList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```