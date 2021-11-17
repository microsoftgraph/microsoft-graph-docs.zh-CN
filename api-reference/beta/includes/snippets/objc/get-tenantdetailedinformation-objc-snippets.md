---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16df8a1ac1a91b61a012037c0b233c37545e56c81dfafbd8049977e7f46d1c8f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215836"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/tenantsDetailedInformation/{tenantDetailedInformationId}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphTenantDetailedInformation *tenantDetailedInformation = [[MSGraphTenantDetailedInformation alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```