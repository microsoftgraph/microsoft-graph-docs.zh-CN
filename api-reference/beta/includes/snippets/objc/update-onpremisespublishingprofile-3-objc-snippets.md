---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a6b1ba458aa151f646c759b25c373d869eb9d91
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963221"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphHybridAgentUpdaterConfiguration *hybridAgentUpdaterConfiguration = [[MSGraphHybridAgentUpdaterConfiguration alloc] init];
[hybridAgentUpdaterConfiguration setAllowUpdateConfigurationOverride: false];

NSError *error;
NSData *hybridAgentUpdaterConfigurationData = [hybridAgentUpdaterConfiguration getSerializedDataWithError:&error];
[urlRequest setHTTPBody:hybridAgentUpdaterConfigurationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```