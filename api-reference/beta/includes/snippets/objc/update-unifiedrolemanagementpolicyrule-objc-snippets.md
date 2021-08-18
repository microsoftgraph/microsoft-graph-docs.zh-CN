---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed2e252ea3c99a4c908e82f3644859cdecff171687b6da3b579358b3292842aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162693"
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