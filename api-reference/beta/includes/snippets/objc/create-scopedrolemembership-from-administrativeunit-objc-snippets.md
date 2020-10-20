---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59654ee87498a2f728340cc872ca1e700b8bb22d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615231"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/administrativeUnits/{id}/scopedRoleMembers"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphScopedRoleMembership *scopedRoleMembership = [[MSGraphScopedRoleMembership alloc] init];
[scopedRoleMembership setRoleId:@"roleId-value"];
MSGraphIdentity *roleMemberInfo = [[MSGraphIdentity alloc] init];
[roleMemberInfo setId:@"id-value"];
[scopedRoleMembership setRoleMemberInfo:roleMemberInfo];

NSError *error;
NSData *scopedRoleMembershipData = [scopedRoleMembership getSerializedDataWithError:&error];
[urlRequest setHTTPBody:scopedRoleMembershipData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```