---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ceb4bcaadb28eaec4046df9821772ffcb409a9aa87b0b3b42532b72a33b6a72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378296"
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