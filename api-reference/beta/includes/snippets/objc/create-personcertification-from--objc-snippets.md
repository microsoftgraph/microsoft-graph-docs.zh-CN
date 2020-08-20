---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1967d2ff4323a81156d560747162e617183c5a93
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820196"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/certifications"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPersonCertification *personCertification = [[MSGraphPersonCertification alloc] init];
[personCertification setCertificationId:@"KB-1235466333663322"];
[personCertification setDescription:@"Blackbelt in Marketing - Brand Management"];
[personCertification setDisplayName:@"Marketing Blackbelt - Brand Management"];
[personCertification setThumbnailUrl:@"https://iame.io/dfhdfdfd334.jpg"];
[personCertification setWebUrl:@"https://www.iame.io/blackbelt"];

NSError *error;
NSData *personCertificationData = [personCertification getSerializedDataWithError:&error];
[urlRequest setHTTPBody:personCertificationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```