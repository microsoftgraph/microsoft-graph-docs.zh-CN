---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3e66e26e4d5a9c61fa2c40af19a5561066959c3
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52663940"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/conditionalAccess/authenticationContextClassReferences"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAuthenticationContextClassReference *authenticationContextClassReference = [[MSGraphAuthenticationContextClassReference alloc] init];
[authenticationContextClassReference setId:@"c1"];
[authenticationContextClassReference setDisplayName:@"Contoso medium"];
[authenticationContextClassReference setDescription:@"Medium protection level defined for Contoso policy"];
[authenticationContextClassReference setIsAvailable: true];

NSError *error;
NSData *authenticationContextClassReferenceData = [authenticationContextClassReference getSerializedDataWithError:&error];
[urlRequest setHTTPBody:authenticationContextClassReferenceData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```