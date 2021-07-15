---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de35af71c6e5e9c5ec38aba8006d2d58cd648b1b
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439141"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageResourceRequests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessPackageResourceRequest *accessPackageResourceRequest = [[MSGraphAccessPackageResourceRequest alloc] init];
[accessPackageResourceRequest setCatalogId:@"beedadfe-01d5-4025-910b-84abb9369997"];
[accessPackageResourceRequest setRequestType:@"AdminAdd"];
MSGraphAccessPackageResource *accessPackageResource = [[MSGraphAccessPackageResource alloc] init];
[accessPackageResource setOriginId:@"c6294667-7348-4f5a-be73-9d2c65f574f3"];
[accessPackageResource setOriginSystem:@"AadGroup"];
[accessPackageResourceRequest setAccessPackageResource:accessPackageResource];

NSError *error;
NSData *accessPackageResourceRequestData = [accessPackageResourceRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessPackageResourceRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```