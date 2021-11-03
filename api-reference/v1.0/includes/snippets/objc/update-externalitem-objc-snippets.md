---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b350ff956261a2e3e9ac05b5544a65bea0499892
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688748"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/external/connections/contosohr/items/TSP228082938"]]];
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