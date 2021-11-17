---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c7892f1eb52c1d2fdc50038f957edf6d2b9d46f0b3672173653a845dc7d31b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104096"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/activityBasedTimeoutPolicies/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
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