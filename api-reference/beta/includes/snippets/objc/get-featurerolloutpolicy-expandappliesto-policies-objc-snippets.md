---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 661b5aa7d83c3ea431b0f9b626d6a766b6bd2d1a640f83267144d9a1574c57e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332939"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphFeatureRolloutPolicy *featureRolloutPolicy = [[MSGraphFeatureRolloutPolicy alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```