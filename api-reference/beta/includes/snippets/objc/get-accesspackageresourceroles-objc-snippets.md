---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 201a2bf2bba3251aa344808a50d33fa963a5ddb73b4a75645489e7797e16e57b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902773"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageCatalogs/15d889df-3eb8-4e9b-bfb4-b1908849aec4/accessPackageResourceRoles?$filter=(originSystem%20eq%20'AadGroup'%20and%20accessPackageResource/id%20eq%20'a35bef72-a8aa-4ca3-af30-f6b2ece7208f')&$expand=accessPackageResource"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphAccessPackageResourceRole *accessPackageResourceRole = [[MSGraphAccessPackageResourceRole alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```