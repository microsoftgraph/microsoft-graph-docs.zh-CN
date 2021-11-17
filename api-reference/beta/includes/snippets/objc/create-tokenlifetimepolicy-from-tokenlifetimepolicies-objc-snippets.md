---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 994723c3fdd44c4353ebc47c633d82f36d39eee8e76305b64cf8f653cbc4e849
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903285"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/tokenLifetimePolicies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTokenLifetimePolicy *tokenLifetimePolicy = [[MSGraphTokenLifetimePolicy alloc] init];
NSMutableArray *definitionList = [[NSMutableArray alloc] init];
[definitionList addObject: @"definition-value"];
[tokenLifetimePolicy setDefinition:definitionList];
[tokenLifetimePolicy setDisplayName:@"displayName-value"];
[tokenLifetimePolicy setIsOrganizationDefault: true];

NSError *error;
NSData *tokenLifetimePolicyData = [tokenLifetimePolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:tokenLifetimePolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```