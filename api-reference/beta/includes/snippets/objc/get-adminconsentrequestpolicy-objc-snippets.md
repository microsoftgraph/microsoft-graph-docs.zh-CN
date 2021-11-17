---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85ac05a8b7a0eb1e4b86d405c5ac71baa95838641d0c4a38e265eece7238e49a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104093"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/adminConsentRequestPolicy"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphAdminConsentRequestPolicy *adminConsentRequestPolicy = [[MSGraphAdminConsentRequestPolicy alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```