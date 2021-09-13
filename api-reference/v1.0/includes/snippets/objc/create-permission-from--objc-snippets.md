---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9197d0fe39553c48210aca4041c94c96a8de5bda213c0fee46ca5ac85069c70
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332329"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{sitesId}/permissions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPermission *permission = [[MSGraphPermission alloc] init];
NSMutableArray *rolesList = [[NSMutableArray alloc] init];
[rolesList addObject: @"write"];
[permission setRoles:rolesList];
NSMutableArray *grantedToIdentitiesList = [[NSMutableArray alloc] init];
MSGraphIdentitySet *grantedToIdentities = [[MSGraphIdentitySet alloc] init];
MSGraphIdentity *application = [[MSGraphIdentity alloc] init];
[application setId:@"89ea5c94-7736-4e25-95ad-3fa95f62b66e"];
[application setDisplayName:@"Contoso Time Manager App"];
[grantedToIdentities setApplication:application];
[grantedToIdentitiesList addObject: grantedToIdentities];
[permission setGrantedToIdentities:grantedToIdentitiesList];

NSError *error;
NSData *permissionData = [permission getSerializedDataWithError:&error];
[urlRequest setHTTPBody:permissionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```