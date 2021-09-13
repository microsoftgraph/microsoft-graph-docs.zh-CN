---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa044c8e253d32495ddf8da84a94c7adf3413a6bfecf2b87e37de588172db9f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220861"
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