---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5078c625f04f6e3a8a65b0394008795df68aa978
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441801"
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