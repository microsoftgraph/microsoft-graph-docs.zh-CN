---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae471001969b0e4f8b327cf9049e0ddbdd7fcb4467e2acdcc7832210d2012a19
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105706"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUnifiedRoleManagementPolicyRule *unifiedRoleManagementPolicyRule = [[MSGraphUnifiedRoleManagementPolicyRule alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```