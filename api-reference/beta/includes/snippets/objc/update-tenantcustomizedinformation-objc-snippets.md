---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24a642ecda1f2bd4e4bb9ca935ff44c6a373ffbba4971026ac4ea071709b6334
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279501"
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