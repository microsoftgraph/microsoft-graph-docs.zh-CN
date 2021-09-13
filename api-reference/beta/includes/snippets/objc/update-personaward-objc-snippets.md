---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6048638656ba46020899678db628ef084aaef3858f503ac6999c76c661a3780c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329011"
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