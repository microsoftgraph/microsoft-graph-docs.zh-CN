---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f701a8c6d5bceba59b66b405d42a446fd9439130299edf4ca6a3499e8a045d1e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104075"
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