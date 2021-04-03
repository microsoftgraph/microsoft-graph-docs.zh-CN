---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fa9a05a15f497b4a60ed90bfee9eec5527dc808
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573207"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/connections/contosohr/items/TSP228082938"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalConnectorsExternalItem *externalItem = [[MSGraphExternalConnectorsExternalItem alloc] init];
NSMutableArray *aclList = [[NSMutableArray alloc] init];
MSGraphExternalConnectorsAcl *acl = [[MSGraphExternalConnectorsAcl alloc] init];
[acl setType: [MSGraphExternalConnectorsAclType everyone]];
[acl setValue:@"67a141d8-cf4e-4528-ba07-bed21bfacd2d"];
[acl setAccessType: [MSGraphExternalConnectorsAccessType grant]];
[acl setIdentitySource: [MSGraphExternalConnectorsIdentitySourceType azureActiveDirectory]];
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