---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5736422eaeb1ded30ba5c9faa1b89adb81ff816e97b9752cd1d812b64af3efda
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104495"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2cUserFlows/{id}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphB2cIdentityUserFlow *b2cIdentityUserFlow = [[MSGraphB2cIdentityUserFlow alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```