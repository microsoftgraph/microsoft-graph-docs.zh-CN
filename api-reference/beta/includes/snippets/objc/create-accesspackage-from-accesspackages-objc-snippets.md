---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3cad76ef3dcb57bdececf85128c56090cd794a89eade8554ba7874f7783b492
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104206"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackages"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessPackage *accessPackage = [[MSGraphAccessPackage alloc] init];
[accessPackage setCatalogId:@"aa2f6514-3232-46e7-a08a-2411ad8d7128"];
[accessPackage setDisplayName:@"sales reps"];
[accessPackage setDescription:@"outside sales representatives"];

NSError *error;
NSData *accessPackageData = [accessPackage getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessPackageData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```