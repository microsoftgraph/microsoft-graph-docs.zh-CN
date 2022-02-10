---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14192c354d2e477736cc4083bfc6fb9daaa384c6
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519649"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/catalogs/{accessPackageCatalogId}"]]];
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