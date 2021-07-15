---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d71b38d57491ed0c3e5c0e2387edd2d1d201d65
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442712"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/tenantTags/{tenantTagId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphManagedTenantsTenantTag *tenantTag = [[MSGraphManagedTenantsTenantTag alloc] init];
[tenantTag setDisplayName:@"Onboarding"];
[tenantTag setDescription:@"Tenants that we are currently onboarding"];

NSError *error;
NSData *tenantTagData = [tenantTag getSerializedDataWithError:&error];
[urlRequest setHTTPBody:tenantTagData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```