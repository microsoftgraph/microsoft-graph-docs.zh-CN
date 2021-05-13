---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c311ecf07024e1d5d9059fd19e10deb080efbe76
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475059"
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