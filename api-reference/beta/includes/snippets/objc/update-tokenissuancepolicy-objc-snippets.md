---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a699823e1e2bf5e0b910e8b28b46286dbc85717b
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910770"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/tokenIssuancePolicies/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTokenIssuancePolicy *tokenIssuancePolicy = [[MSGraphTokenIssuancePolicy alloc] init];
NSMutableArray *definitionList = [[NSMutableArray alloc] init];
[definitionList addObject: @"definition-value"];
[tokenIssuancePolicy setDefinition:definitionList];
[tokenIssuancePolicy setDisplayName:@"displayName-value"];
[tokenIssuancePolicy setIsOrganizationDefault: true];

NSError *error;
NSData *tokenIssuancePolicyData = [tokenIssuancePolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:tokenIssuancePolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```