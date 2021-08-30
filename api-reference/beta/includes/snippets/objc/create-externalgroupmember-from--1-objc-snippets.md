---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3af6f0a6760f3d926cfec466c3cacde97198294285a75d90394faf8a8e5fe4d0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215893"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/external/connections/contosohr/groups/31bea3d537902000/members"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalConnectorsExternalGroupMember *externalGroupMember = [[MSGraphExternalConnectorsExternalGroupMember alloc] init];
[externalGroupMember setId:@"e811976d-83df-4cbd-8b9b-5215b18aa874"];
[externalGroupMember setType: [MSGraphExternalConnectorsExternalGroupMemberType user]];
[externalGroupMember setIdentitySource: [MSGraphExternalConnectorsIdentitySourceType azureActiveDirectory]];

NSError *error;
NSData *externalGroupMemberData = [externalGroupMember getSerializedDataWithError:&error];
[urlRequest setHTTPBody:externalGroupMemberData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```