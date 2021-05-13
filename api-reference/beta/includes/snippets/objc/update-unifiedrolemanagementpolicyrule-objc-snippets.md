---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ead6b31e9372243367b53200132b2ece6ae722b
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474249"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUnifiedRoleManagementPolicyRule *unifiedRoleManagementPolicyRule = [[MSGraphUnifiedRoleManagementPolicyRule alloc] init];
MSGraphUnifiedRoleManagementPolicyRuleTarget *target = [[MSGraphUnifiedRoleManagementPolicyRuleTarget alloc] init];
[unifiedRoleManagementPolicyRule setTarget:target];

NSError *error;
NSData *unifiedRoleManagementPolicyRuleData = [unifiedRoleManagementPolicyRule getSerializedDataWithError:&error];
[urlRequest setHTTPBody:unifiedRoleManagementPolicyRuleData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```