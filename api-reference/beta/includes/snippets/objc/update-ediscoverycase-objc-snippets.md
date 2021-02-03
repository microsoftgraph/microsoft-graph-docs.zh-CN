---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f15a31b354efb0d6c0787f6a30b01e06a729a4be
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093644"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoveryCase *case = [[MSGraphEdiscoveryCase alloc] init];
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