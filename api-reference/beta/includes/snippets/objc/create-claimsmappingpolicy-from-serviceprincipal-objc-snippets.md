---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ede2d52f176463a73ffa13bfdd021eadbdbe4ea9
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767169"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{servicePrincipal-id}/claimsMappingPolicies/$ref"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphClaimsMappingPolicy *claimsMappingPolicy = [[MSGraphClaimsMappingPolicy alloc] init];

NSError *error;
NSData *claimsMappingPolicyData = [claimsMappingPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:claimsMappingPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```