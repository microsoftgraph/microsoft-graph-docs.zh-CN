---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4acc5e1f9bdfaf0c7abfde2d8f13f874963d685a
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573211"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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