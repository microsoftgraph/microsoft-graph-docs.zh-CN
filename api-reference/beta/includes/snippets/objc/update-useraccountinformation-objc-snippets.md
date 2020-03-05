---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 642f5639d547e6f2ac29e1868c094b0d553d6116
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996239"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/account/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUserAccountInformation *userAccountInformation = [[MSGraphUserAccountInformation alloc] init];
[userAccountInformation setAgeGroup:@"ageGroup-value"];
[userAccountInformation setCountryCode:@"countryCode-value"];
MSGraphLocaleInfo *preferredLanguageTag = [[MSGraphLocaleInfo alloc] init];
[preferredLanguageTag setLocale:@"locale-value"];
[preferredLanguageTag setDisplayName:@"displayName-value"];
[userAccountInformation setPreferredLanguageTag:preferredLanguageTag];
[userAccountInformation setUserPrincipalName:@"userPrincipalName-value"];

NSError *error;
NSData *userAccountInformationData = [userAccountInformation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:userAccountInformationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```