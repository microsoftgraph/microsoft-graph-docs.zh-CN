---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc80b1622d4023836a0c7f20b78ccd605ad225af
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346709"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/connectedOrganizations/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphConnectedOrganization *connectedOrganization = [[MSGraphConnectedOrganization alloc] init];
[connectedOrganization setDisplayName:@"Connected organization new name"];
[connectedOrganization setDescription:@"Connected organization new description"];
[connectedOrganization setState: [MSGraphConnectedOrganizationState configured]];

NSError *error;
NSData *connectedOrganizationData = [connectedOrganization getSerializedDataWithError:&error];
[urlRequest setHTTPBody:connectedOrganizationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```