---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd50d541e83b8a8536d83aac7fae1447fc4a290486ea5ff3d9843d5f6125a4a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378310"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/activityBasedTimeoutPolicies/{id}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphActivityBasedTimeoutPolicy *activityBasedTimeoutPolicy = [[MSGraphActivityBasedTimeoutPolicy alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```