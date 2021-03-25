---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76dcabe7e7457064ae7faccff9114043fc7c1262
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201721"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/appConsent/appConsentRequests/af330b30-dd59-4482-a848-0fd81b0438ed"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphAppConsentRequest *appConsentRequest = [[MSGraphAppConsentRequest alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```