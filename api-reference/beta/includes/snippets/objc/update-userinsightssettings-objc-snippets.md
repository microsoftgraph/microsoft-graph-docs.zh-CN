---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1652e8c0156225a171663345dc83c6d1b9d7fe17e2a6ef2615f1ad5336d74688
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164059"
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