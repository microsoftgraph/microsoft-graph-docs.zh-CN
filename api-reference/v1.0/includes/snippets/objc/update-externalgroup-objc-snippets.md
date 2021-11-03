---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65995abb6ff7d985aeabe0975429bbe457a9cf94
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687801"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/external/connections/{connectionsId}/groups/{externalGroupId}"]]];
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