---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 993e2163b40548d2c9109eac83013de777bd6d69
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022647"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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