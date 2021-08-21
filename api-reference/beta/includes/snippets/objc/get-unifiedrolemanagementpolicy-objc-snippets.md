---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19c78ed1cedd3415d9ec7fed9356324a6db6e9d1f6f92fce2747a61beec7fce0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219842"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/roleManagementPolicies/f93a5c37-5c37-f93a-375c-3af9375c3af9"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUnifiedRoleManagementPolicy *unifiedRoleManagementPolicy = [[MSGraphUnifiedRoleManagementPolicy alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```