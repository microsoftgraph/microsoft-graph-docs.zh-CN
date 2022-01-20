---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a95d7ec2d10bdf72c45661389f1c84059a5035f9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137672"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/external/connections/contosohr/groups/31bea3d537902000/members"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalConnectorsIdentity *identity = [[MSGraphExternalConnectorsIdentity alloc] init];
[identity setId:@"1431b9c38ee647f6a"];
[identity setType: [MSGraphExternalConnectorsIdentityType externalGroup]];

NSError *error;
NSData *identityData = [identity getSerializedDataWithError:&error];
[urlRequest setHTTPBody:identityData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```