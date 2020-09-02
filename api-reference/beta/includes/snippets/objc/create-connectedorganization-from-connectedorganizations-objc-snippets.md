---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d4f491f5e38b28c49cb1dede5c7049bb9e52d9f
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47331088"
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
[connectedOrganization setState:@"proposed"];

NSError *error;
NSData *connectedOrganizationData = [connectedOrganization getSerializedDataWithError:&error];
[urlRequest setHTTPBody:connectedOrganizationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```