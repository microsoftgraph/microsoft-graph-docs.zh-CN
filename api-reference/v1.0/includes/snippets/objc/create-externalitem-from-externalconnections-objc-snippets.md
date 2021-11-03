---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5f0a0041af517db49a93bf47fe58ea951eb64eb
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688115"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/external/connections/contosohr/items/TSP228082938"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalConnectorsExternalItem *externalItem = [[MSGraphExternalConnectorsExternalItem alloc] init];
NSMutableArray *aclList = [[NSMutableArray alloc] init];
MSGraphExternalConnectorsAcl *acl = [[MSGraphExternalConnectorsAcl alloc] init];
[acl setType: [MSGraphExternalConnectorsAclType user]];
[acl setValue:@"e811976d-83df-4cbd-8b9b-5215b18aa874"];
[acl setAccessType: [MSGraphExternalConnectorsAccessType grant]];
[aclList addObject: acl];
MSGraphExternalConnectorsAcl *acl = [[MSGraphExternalConnectorsAcl alloc] init];
[acl setType: [MSGraphExternalConnectorsAclType externalGroup]];
[acl setValue:@"14m1b9c38qe647f6a"];
[acl setAccessType: [MSGraphExternalConnectorsAccessType deny]];
[aclList addObject: acl];
[externalItem setAcl:aclList];
MSGraphExternalConnectorsProperties *properties = [[MSGraphExternalConnectorsProperties alloc] init];
[properties setTitle:@"Error in the payment gateway"];
[properties setPriority: 1];
[properties setAssignee:@"john@contoso.com"];
[externalItem setProperties:properties];
MSGraphExternalConnectorsExternalItemContent *content = [[MSGraphExternalConnectorsExternalItemContent alloc] init];
[content setValue:@"Error in payment gateway..."];
[content setType: [MSGraphExternalConnectorsExternalItemContentType text]];
[externalItem setContent:content];

NSError *error;
NSData *externalItemData = [externalItem getSerializedDataWithError:&error];
[urlRequest setHTTPBody:externalItemData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```