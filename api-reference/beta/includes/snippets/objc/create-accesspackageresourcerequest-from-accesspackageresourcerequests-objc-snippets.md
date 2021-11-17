---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 648c51e4a24b988112ec3aabebbe46daf5484b6c72b43a283edb959076368f72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104172"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageResourceRequests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessPackageResourceRequest *accessPackageResourceRequest = [[MSGraphAccessPackageResourceRequest alloc] init];
[accessPackageResourceRequest setCatalogId:@"26ac0c0a-08bc-4a7b-a313-839f58044ba5"];
[accessPackageResourceRequest setRequestType:@"AdminAdd"];
[accessPackageResourceRequest setJustification:@""];
MSGraphAccessPackageResource *accessPackageResource = [[MSGraphAccessPackageResource alloc] init];
[accessPackageResource setDisplayName:@"Sales"];
[accessPackageResource setDescription:@"https://contoso.sharepoint.com/sites/Sales"];
[accessPackageResource setUrl:@"https://contoso.sharepoint.com/sites/Sales"];
[accessPackageResource setResourceType:@"SharePoint Online Site"];
[accessPackageResource setOriginId:@"https://contoso.sharepoint.com/sites/Sales"];
[accessPackageResource setOriginSystem:@"SharePointOnline"];
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