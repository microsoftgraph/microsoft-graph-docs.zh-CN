---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4a544fee12a13a3b5efbc1a20910f90811883db9686732ab73f7e5dd8ccac11
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902787"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphAccessPackageAssignmentResourceRole *accessPackageAssignmentResourceRole = [[MSGraphAccessPackageAssignmentResourceRole alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```