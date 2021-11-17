---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a484afb77aaccc050ff77a0cfa50f8ed76134c7657c8ed788fdd84a9f0d9127
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902817"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphAccessPackageAssignmentPolicy *accessPackageAssignmentPolicy = [[MSGraphAccessPackageAssignmentPolicy alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```