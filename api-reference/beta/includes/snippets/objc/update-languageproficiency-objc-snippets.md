---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 372ed6eca766719c4e22ad51d2cc0daeaeed95f2
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998241"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/languages/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphLanguageProficiency *languageProficiency = [[MSGraphLanguageProficiency alloc] init];
[languageProficiency setDisplayName:@"displayName-value"];
[languageProficiency setTag:@"tag-value"];
[languageProficiency setProficiency: [MSGraphLanguageProficiencyLevel elementary]];

NSError *error;
NSData *languageProficiencyData = [languageProficiency getSerializedDataWithError:&error];
[urlRequest setHTTPBody:languageProficiencyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```