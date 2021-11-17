---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 565c1001540b5dcd71c4c6a473cec7bdbaa2e9f3e4a4931e87719389c1a37037
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278447"
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