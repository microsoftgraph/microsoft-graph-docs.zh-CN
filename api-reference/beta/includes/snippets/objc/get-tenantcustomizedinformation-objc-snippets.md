---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fae8bbbeaf4fd9f2375764e37cf5ab9b36b1164acc3d4903037d9861a7a72c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161408"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphTenantCustomizedInformation *tenantCustomizedInformation = [[MSGraphTenantCustomizedInformation alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```