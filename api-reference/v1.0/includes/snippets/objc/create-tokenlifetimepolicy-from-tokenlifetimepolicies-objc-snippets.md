---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 264d85d1b2c379ce123994b1320d87fb9bc256ccd9c11c8001f2c1be3b48aba3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220355"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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