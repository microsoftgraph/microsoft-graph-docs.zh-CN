---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22019382a520cd9247e4cf57daeb4afe4f7f1923
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956016"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/external/connections/contosohr/groups/31bea3d537902000/members"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalGroupMember *externalGroupMember = [[MSGraphExternalGroupMember alloc] init];
[externalGroupMember setId:@"1431b9c38ee647f6a"];
[externalGroupMember setType: [MSGraphExternalGroupMemberType group]];
[externalGroupMember setIdentitySource: [MSGraphIdentitySourceType external]];

NSError *error;
NSData *externalGroupMemberData = [externalGroupMember getSerializedDataWithError:&error];
[urlRequest setHTTPBody:externalGroupMemberData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```