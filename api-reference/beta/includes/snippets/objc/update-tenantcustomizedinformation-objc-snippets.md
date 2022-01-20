---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe4eae957f2b2a687ef3a888dda232f62ef244bf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137683"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphManagedTenantsTenantCustomizedInformation *tenantCustomizedInformation = [[MSGraphManagedTenantsTenantCustomizedInformation alloc] init];
[tenantCustomizedInformation setTenantId:@"String"];
NSMutableArray *contactsList = [[NSMutableArray alloc] init];
MSGraphManagedTenantsTenantContactInformation *contacts = [[MSGraphManagedTenantsTenantContactInformation alloc] init];
[contacts setName:@"String"];
[contacts setTitle:@"String"];
[contacts setEmail:@"String"];
[contacts setPhone:@"String"];
[contacts setNotes:@"String"];
[contactsList addObject: contacts];
[tenantCustomizedInformation setContacts:contactsList];
[tenantCustomizedInformation setWebsite:@"String"];

NSError *error;
NSData *tenantCustomizedInformationData = [tenantCustomizedInformation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:tenantCustomizedInformationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```