---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed5a8edff85fc4ae5970db21099139726c1f0330cbe31de0a3b5dcb84dc0b9ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104169"
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