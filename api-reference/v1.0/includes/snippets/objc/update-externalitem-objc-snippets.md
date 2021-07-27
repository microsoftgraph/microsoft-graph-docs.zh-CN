---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6cf27197180f20a22b2da65205d69af81b1f352
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580751"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/connections/contosohr/items/TSP228082938"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalConnectorsExternalItem *externalItem = [[MSGraphExternalConnectorsExternalItem alloc] init];
NSMutableArray *aclList = [[NSMutableArray alloc] init];
MSGraphExternalConnectorsAcl *acl = [[MSGraphExternalConnectorsAcl alloc] init];
[acl setType: [MSGraphExternalConnectorsAclType everyone]];
[acl setValue:@"67a141d8-cf4e-4528-ba07-bed21bfacd2d"];
[acl setAccessType: [MSGraphExternalConnectorsAccessType grant]];
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