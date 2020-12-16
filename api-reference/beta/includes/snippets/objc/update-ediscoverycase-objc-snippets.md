---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9bbe4901c645664040afab4f91681a1ce56c040
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692808"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCase *case = [[MSGraphCase alloc] init];
[case setDisplayName:@"My Case 1 - Renamed"];
[case setDescription:@"Updated description"];
[case setExternalId:@"Updated externalId"];

NSError *error;
NSData *caseData = [case getSerializedDataWithError:&error];
[urlRequest setHTTPBody:caseData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```