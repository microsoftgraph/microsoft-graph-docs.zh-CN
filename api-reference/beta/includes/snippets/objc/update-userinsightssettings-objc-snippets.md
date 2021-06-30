---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0e178f681559b8ba4292c076e572467990dfad3
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210658"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{userId}/settings/itemInsights"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUserInsightsSettings *userInsightsSettings = [[MSGraphUserInsightsSettings alloc] init];
[userInsightsSettings setIsEnabled:@"false"];

NSError *error;
NSData *userInsightsSettingsData = [userInsightsSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:userInsightsSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```