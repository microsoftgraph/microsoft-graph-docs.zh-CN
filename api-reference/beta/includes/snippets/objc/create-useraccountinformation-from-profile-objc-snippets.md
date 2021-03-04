---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d2fa2ecc792c94346067ea8deff0f4706a36157c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441008"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/account"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUserAccountInformation *userAccountInformation = [[MSGraphUserAccountInformation alloc] init];
[userAccountInformation setAllowedAudiences: [MSGraphAllowedAudiences organization]];
[userAccountInformation setCountryCode:@"NO"];

NSError *error;
NSData *userAccountInformationData = [userAccountInformation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:userAccountInformationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```