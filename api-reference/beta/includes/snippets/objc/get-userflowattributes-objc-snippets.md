---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1861d5a1f927ca5aa4468ccf1db0db60c56e4c0814138f0e8ab79b77987b577
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332293"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/userFlowAttributes/{id}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphIdentityUserFlowAttribute *identityUserFlowAttribute = [[MSGraphIdentityUserFlowAttribute alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```