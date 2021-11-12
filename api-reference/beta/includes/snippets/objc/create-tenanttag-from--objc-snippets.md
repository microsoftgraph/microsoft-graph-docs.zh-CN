---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eecad58ab4f90a92039d02714681b6bf117fc595922e3cb0b418ecfd14765b7e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158524"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/tenantTags"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphManagedTenantsTenantTag *tenantTag = [[MSGraphManagedTenantsTenantTag alloc] init];
[tenantTag setDisplayName:@"Support"];
[tenantTag setDescription:@"Tenants that have purchased extended support"];

NSError *error;
NSData *tenantTagData = [tenantTag getSerializedDataWithError:&error];
[urlRequest setHTTPBody:tenantTagData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```