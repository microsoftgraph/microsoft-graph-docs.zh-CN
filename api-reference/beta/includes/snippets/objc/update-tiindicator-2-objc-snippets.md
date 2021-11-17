---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f789b333fd34dd07228d0fb3e72ba36a9682c7d9de9da638e0d67bbf32fd435
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220193"
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