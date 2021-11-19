---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9402b41fd7732d297b5d365607a8eaf60fbaceb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102153"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization/{organizationId}/settings/itemInsights"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphInsightsSettings *insightsSettings = [[MSGraphInsightsSettings alloc] init];
[insightsSettings setDisabledForGroup:@"edbfe4fb-ec70-4300-928f-dbb2ae86c981"];

NSError *error;
NSData *insightsSettingsData = [insightsSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:insightsSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```