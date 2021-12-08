---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b11570115fcfcb24ff76ba232308170307ddb16
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347971"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/connectedOrganizations/"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphConnectedOrganization *connectedOrganization = [[MSGraphConnectedOrganization alloc] init];
[connectedOrganization setDisplayName:@"Connected organization name"];
[connectedOrganization setDescription:@"Connected organization description"];
NSMutableArray *identitySourcesList = [[NSMutableArray alloc] init];
MSGraphIdentitySource *identitySources = [[MSGraphIdentitySource alloc] init];
[identitySources setDomainName:@"example.com"];
[identitySources setDisplayName:@"example.com"];
[identitySourcesList addObject: identitySources];
[connectedOrganization setIdentitySources:identitySourcesList];
[connectedOrganization setState: [MSGraphConnectedOrganizationState proposed]];

NSError *error;
NSData *connectedOrganizationData = [connectedOrganization getSerializedDataWithError:&error];
[urlRequest setHTTPBody:connectedOrganizationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```