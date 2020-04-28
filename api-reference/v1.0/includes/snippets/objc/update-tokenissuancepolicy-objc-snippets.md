---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33c80b865c10c24d936a0fa32b62060c291dc267
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719453"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/tokenIssuancePolicies/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTokenIssuancePolicy *tokenIssuancePolicy = [[MSGraphTokenIssuancePolicy alloc] init];
NSMutableArray *definitionList = [[NSMutableArray alloc] init];
[definitionList addObject: @"definition-value"];
[tokenIssuancePolicy setDefinition:definitionList];
[tokenIssuancePolicy setDisplayName:@"displayName-value"];
[tokenIssuancePolicy setIsOrganizationDefault: true];
[tokenIssuancePolicy setType:@"type-value"];

NSError *error;
NSData *tokenIssuancePolicyData = [tokenIssuancePolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:tokenIssuancePolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```