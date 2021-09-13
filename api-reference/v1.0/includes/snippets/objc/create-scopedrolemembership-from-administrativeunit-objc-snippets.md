---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be502dce1bb3a5212212233b38ebec999d41d14a56eac1ee9e660306b935cea5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105436"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directory/administrativeUnits/{id}/scopedRoleMembers"]]];
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