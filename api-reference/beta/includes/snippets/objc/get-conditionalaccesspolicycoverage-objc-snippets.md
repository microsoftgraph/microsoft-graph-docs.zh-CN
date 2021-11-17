---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14668bd331ddf7fcd09c79ddc344143a3d2b4df1e25754e6d5c4668b3112dd0e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221519"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/conditionalAccessPolicyCoverages/{conditionalAccessPolicyCoverageId}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphConditionalAccessPolicyCoverage *conditionalAccessPolicyCoverage = [[MSGraphConditionalAccessPolicyCoverage alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```