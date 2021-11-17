---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f784b324fe914179767c574decba2fe01eacb1875ec7490af4497c9ca56ba136
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104052"
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