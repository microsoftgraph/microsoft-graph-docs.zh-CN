---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8aea1e230ed253e0a368a5853e16be958b1950263f8096f89500051724447c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332373"
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