---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec6ecfd988a6206f94348e7c58d558509d123dc7
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567064"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization/{organizationId}/settings/itemInsights"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphItemInsightsSettings *itemInsightsSettings = [[MSGraphItemInsightsSettings alloc] init];
[itemInsightsSettings setDisabledForGroup:@"edbfe4fb-ec70-4300-928f-dbb2ae86c981"];

NSError *error;
NSData *itemInsightsSettingsData = [itemInsightsSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:itemInsightsSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```