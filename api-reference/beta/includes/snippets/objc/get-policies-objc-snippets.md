---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de618afa7029d30de28ce3c68183e1dca4702fa7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936654"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/conditionalAccess/policies?$filter=displayName%20eq%20'SimplePolicy1'%20or%20displayName%20eq%20'SimplePolicy2'"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *conditionalAccessPolicyList = [[NSMutableArray alloc] init];
        conditionalAccessPolicyList = [jsonFinal valueForKey:@"value"];
        MSGraphConditionalAccessPolicy *conditionalAccessPolicy = [[MSGraphConditionalAccessPolicy alloc] initWithDictionary:[conditionalAccessPolicyList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```