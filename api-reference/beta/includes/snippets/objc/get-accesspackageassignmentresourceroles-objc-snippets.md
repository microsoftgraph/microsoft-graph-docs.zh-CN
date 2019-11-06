---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ee693fd301d3eace0ceff4d5f7fcc045ab9f963
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994299"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *accessPackageAssignmentResourceRoleList = [[NSMutableArray alloc] init];
        accessPackageAssignmentResourceRoleList = [jsonFinal valueForKey:@"value"];
        MSGraphAccessPackageAssignmentResourceRole *accessPackageAssignmentResourceRole = [[MSGraphAccessPackageAssignmentResourceRole alloc] initWithDictionary:[accessPackageAssignmentResourceRoleList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```