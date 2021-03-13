---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85dd9143bf4189ecfb191b77a7f60f37f9639d77
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774122"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{userId}/profile/awards/{personAwardId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPersonAward *personAward = [[MSGraphPersonAward alloc] init];
[personAward setIssuingAuthority:@"International Association of Branding Management"];
[personAward setThumbnailUrl:@"https://iabm.io/sdhdfhsdhshsd.jpg"];

NSError *error;
NSData *personAwardData = [personAward getSerializedDataWithError:&error];
[urlRequest setHTTPBody:personAwardData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```