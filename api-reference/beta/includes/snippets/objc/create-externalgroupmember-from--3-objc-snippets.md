---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be6f19004596eb342ee2e9e14207aef3e21e8ab7
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573199"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/external/connections/contosohr/groups/31bea3d537902000/members"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalConnectorsExternalGroupMember *externalGroupMember = [[MSGraphExternalConnectorsExternalGroupMember alloc] init];
[externalGroupMember setId:@"1431b9c38ee647f6a"];
[externalGroupMember setType: [MSGraphExternalConnectorsExternalGroupMemberType group]];
[externalGroupMember setIdentitySource: [MSGraphExternalConnectorsIdentitySourceType external]];

NSError *error;
NSData *externalGroupMemberData = [externalGroupMember getSerializedDataWithError:&error];
[urlRequest setHTTPBody:externalGroupMemberData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```