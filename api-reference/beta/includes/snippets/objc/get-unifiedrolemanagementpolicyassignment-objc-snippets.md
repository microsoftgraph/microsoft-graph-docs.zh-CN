---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a06bc82bdd3efbcaefd50c5d51363c31ed26f6645e29d82a9648e80e5a673eaf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106246"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/roleManagementPolicyAssignments/d6e4112f-112f-d6e4-2f11-e4d62f11e4d6"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUnifiedRoleManagementPolicyAssignment *unifiedRoleManagementPolicyAssignment = [[MSGraphUnifiedRoleManagementPolicyAssignment alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```