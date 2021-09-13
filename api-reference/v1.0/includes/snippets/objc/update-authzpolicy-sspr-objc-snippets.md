---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6224910d65b3c5345a4de6bee6dd68e1672771b94030b15f064fbba18febd38b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332204"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/authorizationPolicy"]]];
[urlRequest setHTTPMethod:@"PATCH"];

MSGraphAuthorizationPolicy *authorizationPolicy = [[MSGraphAuthorizationPolicy alloc] init];
[authorizationPolicy setAllowedToUseSSPR: true];

NSError *error;
NSData *authorizationPolicyData = [authorizationPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:authorizationPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```