---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f02164caad5a3ddb74953482c39b5983422e804e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992883"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessPackageAssignmentPolicy *accessPackageAssignmentPolicy = [[MSGraphAccessPackageAssignmentPolicy alloc] init];
[accessPackageAssignmentPolicy setAccessPackageId:@"56ff43fd-6b05-48df-9634-956a777fce6d"];
[accessPackageAssignmentPolicy setDisplayName:@"direct"];
[accessPackageAssignmentPolicy setDescription:@"direct assignments by administrator"];
[accessPackageAssignmentPolicy setIsEnabled: true];

NSError *error;
NSData *accessPackageAssignmentPolicyData = [accessPackageAssignmentPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessPackageAssignmentPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```