---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 934c94b6b7653a6a6fa4d68196756213cc291ef0b7ad1a87ec0e2cdb5343eaf2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104229"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackages/{id}?$expand=accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphAccessPackage *accessPackage = [[MSGraphAccessPackage alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```