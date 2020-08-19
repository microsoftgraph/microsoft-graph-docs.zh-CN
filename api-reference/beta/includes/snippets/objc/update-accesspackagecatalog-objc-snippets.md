---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 472c2699d73f5df74150a448162037c38d856004
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806416"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessPackageCatalog *accessPackageCatalog = [[MSGraphAccessPackageCatalog alloc] init];
[accessPackageCatalog setDisplayName:@"Catalog One"];

NSError *error;
NSData *accessPackageCatalogData = [accessPackageCatalog getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessPackageCatalogData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```