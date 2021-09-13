---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2afce15df92ebf6cf57140424b6ea1a3db33a87fcf1f09b5fd19d848dea884d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278920"
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