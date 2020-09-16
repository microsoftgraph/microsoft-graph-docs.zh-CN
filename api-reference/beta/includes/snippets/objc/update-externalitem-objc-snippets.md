---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 354a137352c1a20815c8c37b763b2b6251666344
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47938402"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/connections/contosohr/items/TSP228082938"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalItem *externalItem = [[MSGraphExternalItem alloc] init];
NSMutableArray *aclList = [[NSMutableArray alloc] init];
MSGraphAcl *acl = [[MSGraphAcl alloc] init];
[acl setType: [MSGraphAclType user]];
[acl setValue:@"49103559-feac-4575-8b94-254814dfca72"];
[acl setAccessType: [MSGraphAccessType grant]];
[acl setIdentitySource:@"azureActiveDirectory"];
[aclList addObject: acl];
[externalItem setAcl:aclList];

NSError *error;
NSData *externalItemData = [externalItem getSerializedDataWithError:&error];
[urlRequest setHTTPBody:externalItemData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```