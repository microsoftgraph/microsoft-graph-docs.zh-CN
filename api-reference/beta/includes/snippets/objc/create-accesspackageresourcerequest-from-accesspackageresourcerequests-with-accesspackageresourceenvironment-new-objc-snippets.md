---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8536c521a73ca6a82fff27465b559f5b5242a002
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176355"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageResourceRequests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessPackageResourceRequest *accessPackageResourceRequest = [[MSGraphAccessPackageResourceRequest alloc] init];
[accessPackageResourceRequest setCatalogId:@"de9315c1-272b-4905-924b-cc112ca180c7"];
MSGraphAccessPackageResource *accessPackageResource = [[MSGraphAccessPackageResource alloc] init];
[accessPackageResource setDisplayName:@"Community Outreach"];
[accessPackageResource setDescription:@"https://contoso.sharepoint.com/sites/CSR"];
[accessPackageResource setResourceType:@"SharePoint Online Site"];
[accessPackageResource setOriginId:@"https://contoso.sharepoint.com/sites/CSR"];
[accessPackageResource setOriginSystem:@"SharePointOnline"];
MSGraphAccessPackageResourceEnvironment *accessPackageResourceEnvironment = [[MSGraphAccessPackageResourceEnvironment alloc] init];
[accessPackageResourceEnvironment setOriginId:@"https://contoso-admin.sharepoint.com/"];
[accessPackageResource setAccessPackageResourceEnvironment:accessPackageResourceEnvironment];
[accessPackageResourceRequest setAccessPackageResource:accessPackageResource];
[accessPackageResourceRequest setRequestType:@"AdminAdd"];

NSError *error;
NSData *accessPackageResourceRequestData = [accessPackageResourceRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessPackageResourceRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```