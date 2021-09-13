---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c086f8507b2192e328458c3f75e06fb00b4597c6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022500"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/external/connections/contosohr/groups"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalConnectorsExternalGroup *externalGroup = [[MSGraphExternalConnectorsExternalGroup alloc] init];
[externalGroup setId:@"31bea3d537902000"];
[externalGroup setDisplayName:@"Contoso Marketing"];
[externalGroup setDescription:@"The product marketing team"];

NSError *error;
NSData *externalGroupData = [externalGroup getSerializedDataWithError:&error];
[urlRequest setHTTPBody:externalGroupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```