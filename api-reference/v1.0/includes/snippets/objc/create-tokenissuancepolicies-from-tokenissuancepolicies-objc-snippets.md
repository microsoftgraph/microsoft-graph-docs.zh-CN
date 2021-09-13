---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d04da35128c111d924399d59a72c1345f9be545f0e505b2c08f6c1984ca74a9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106762"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/tokenIssuancePolicies"]]];
[urlRequest setHTTPMethod:@"POST"];
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