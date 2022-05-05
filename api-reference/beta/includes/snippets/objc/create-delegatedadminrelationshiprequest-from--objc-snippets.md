---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97440b990c3309686307024c08be60a1184209c8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203467"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836/requests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDelegatedAdminRelationshipRequest *delegatedAdminRelationshipRequest = [[MSGraphDelegatedAdminRelationshipRequest alloc] init];
[delegatedAdminRelationshipRequest setAction: [MSGraphDelegatedAdminRelationshipRequestAction lockForApproval]];

NSError *error;
NSData *delegatedAdminRelationshipRequestData = [delegatedAdminRelationshipRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:delegatedAdminRelationshipRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```