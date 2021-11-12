---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7872631558c13fd4092f2611906493baf824354b589561284eb93757e5c5a4fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220803"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphPasswordlessMicrosoftAuthenticatorAuthenticationMethod *passwordlessMicrosoftAuthenticatorAuthenticationMethod = [[MSGraphPasswordlessMicrosoftAuthenticatorAuthenticationMethod alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```