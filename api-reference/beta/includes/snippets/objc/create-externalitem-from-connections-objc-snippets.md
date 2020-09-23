---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b1f24cc3084f91b8cf17f09c0b1cd9a0080a6a8
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48230674"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/connections/contosohr/items/TSP228082938"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalItem *externalItem = [[MSGraphExternalItem alloc] init];
NSMutableArray *aclList = [[NSMutableArray alloc] init];
MSGraphAcl *acl = [[MSGraphAcl alloc] init];
[acl setType: [MSGraphAclType user]];
[acl setValue:@"e811976d-83df-4cbd-8b9b-5215b18aa874"];
[acl setAccessType: [MSGraphAccessType grant]];
[acl setIdentitySource:@"azureActiveDirectory"];
[aclList addObject: acl];
MSGraphAcl *acl = [[MSGraphAcl alloc] init];
[acl setType: [MSGraphAclType group]];
[acl setValue:@"14m1b9c38qe647f6a"];
[acl setAccessType: [MSGraphAccessType deny]];
[acl setIdentitySource:@"external"];
[aclList addObject: acl];
[externalItem setAcl:aclList];
MSGraphProperties *properties = [[MSGraphProperties alloc] init];
[properties setTitle:@"Error in the payment gateway"];
[properties setPriority: 1];
[properties setAssignee:@"john@contoso.com"];
[externalItem setProperties:properties];
MSGraphExternalItemContent *content = [[MSGraphExternalItemContent alloc] init];
[content setValue:@"Error in payment gateway..."];
[content setType: [MSGraphExternalItemContentType text]];
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