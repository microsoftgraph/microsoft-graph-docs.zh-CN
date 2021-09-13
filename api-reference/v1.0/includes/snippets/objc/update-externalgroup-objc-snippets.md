---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ee75aaf4c34288667ad47334fb5690f52b04492
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022370"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/connections/{connectionsId}/groups/{externalGroupId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalConnectorsExternalGroup *externalGroup = [[MSGraphExternalConnectorsExternalGroup alloc] init];
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