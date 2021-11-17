---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d8da4c13f4bcdc36f4242470619049efd06b77edb5164b7a635bb700aab9fe6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105140"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/languages/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphLanguageProficiency *languageProficiency = [[MSGraphLanguageProficiency alloc] init];
[languageProficiency setAllowedAudiences: [MSGraphAllowedAudiences organization]];

NSError *error;
NSData *languageProficiencyData = [languageProficiency getSerializedDataWithError:&error];
[urlRequest setHTTPBody:languageProficiencyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```