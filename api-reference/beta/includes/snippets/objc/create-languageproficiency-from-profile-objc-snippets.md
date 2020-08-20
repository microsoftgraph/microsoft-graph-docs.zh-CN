---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd31f1e16386f2e28ac5c570f78b41d969c92921
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821392"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/languages"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphLanguageProficiency *languageProficiency = [[MSGraphLanguageProficiency alloc] init];
[languageProficiency setDisplayName:@"Norwegian Bokmål"];
[languageProficiency setTag:@"nb-NO"];
[languageProficiency setSpoken: [MSGraphLanguageProficiencyLevel nativeOrBilingual]];
[languageProficiency setWritten: [MSGraphLanguageProficiencyLevel nativeOrBilingual]];
[languageProficiency setReading: [MSGraphLanguageProficiencyLevel nativeOrBilingual]];

NSError *error;
NSData *languageProficiencyData = [languageProficiency getSerializedDataWithError:&error];
[urlRequest setHTTPBody:languageProficiencyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```