---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 362d45267d49ef3061ccdea613e96b39b974724848cb2c18e3278a0d63b7e9c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221521"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{userId}/profile/publications/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphItemPublication *itemPublication = [[MSGraphItemPublication alloc] init];
[itemPublication setPublisher:@"International Association of Branding Management Publishing"];
[itemPublication setThumbnailUrl:@"https://iabm.io/sdhdfhsdhshsd.jpg"];

NSError *error;
NSData *itemPublicationData = [itemPublication getSerializedDataWithError:&error];
[urlRequest setHTTPBody:itemPublicationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```