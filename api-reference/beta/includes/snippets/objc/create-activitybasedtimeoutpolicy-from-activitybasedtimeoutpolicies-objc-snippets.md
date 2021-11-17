---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39560d1029b064a525846cbdc1401215c90fe0250303b3f5aacb98fedf3ed22d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104101"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/activityBasedTimeoutPolicies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphActivityBasedTimeoutPolicy *activityBasedTimeoutPolicy = [[MSGraphActivityBasedTimeoutPolicy alloc] init];
NSMutableArray *definitionList = [[NSMutableArray alloc] init];
[definitionList addObject: @"definition-value"];
[activityBasedTimeoutPolicy setDefinition:definitionList];
[activityBasedTimeoutPolicy setDisplayName:@"displayName-value"];
[activityBasedTimeoutPolicy setIsOrganizationDefault: true];

NSError *error;
NSData *activityBasedTimeoutPolicyData = [activityBasedTimeoutPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:activityBasedTimeoutPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```