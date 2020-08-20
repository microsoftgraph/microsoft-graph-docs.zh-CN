---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c2d0497c8eea02fc4457ba0f2b3fc25ae0e8f0d
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819562"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/awards"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPersonAward *personAward = [[MSGraphPersonAward alloc] init];
[personAward setDescription:@"Lifetime Achievement award from the International Association of Branding Managers"];
[personAward setDisplayName:@"Lifetime Achievement Award For Excellence in Branding"];
[personAward setIssuedDate:@"Date"];
[personAward setIssuingAuthority:@"International Association of Branding Management"];
[personAward setThumbnailUrl:@"https://iabm.io/sdhdfhsdhshsd.jpg"];
[personAward setWebUrl:@"https://www.iabm.io"];

NSError *error;
NSData *personAwardData = [personAward getSerializedDataWithError:&error];
[urlRequest setHTTPBody:personAwardData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```