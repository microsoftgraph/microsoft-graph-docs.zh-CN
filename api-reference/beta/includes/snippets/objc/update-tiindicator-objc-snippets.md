---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 79ada738f4b8f2e3fe9b6aa773083eec45f621e3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520557"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/security/tiIndicators/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"return=representation" forHTTPHeaderField:@"Prefer"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTiIndicator *tiIndicator = [[MSGraphTiIndicator alloc] init];
[tiIndicator setAdditionalInformation:@"additionalInformation-after-update"];
[tiIndicator setConfidence: 42];
[tiIndicator setDescription:@"description-after-update"];

NSError *error;
NSData *tiIndicatorData = [tiIndicator getSerializedDataWithError:&error];
[urlRequest setHTTPBody:tiIndicatorData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```