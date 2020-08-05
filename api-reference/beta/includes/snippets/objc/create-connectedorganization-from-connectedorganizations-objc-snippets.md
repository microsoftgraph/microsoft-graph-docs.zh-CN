---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 729fc1bf28f86f7e44a62ccb1bd28b71c75b6852
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566532"
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

NSError *error;
NSData *connectedOrganizationData = [connectedOrganization getSerializedDataWithError:&error];
[urlRequest setHTTPBody:connectedOrganizationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```