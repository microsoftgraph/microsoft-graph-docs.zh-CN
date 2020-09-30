---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b127de0e8fdd4307169bffd8b0daf0bdc090b7c7
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48317955"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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