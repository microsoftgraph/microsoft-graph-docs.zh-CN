---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94f1e95a2247e2f6dee8bae90d26ba79baa9220a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963218"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphHybridAgentUpdaterConfiguration *hybridAgentUpdaterConfiguration = [[MSGraphHybridAgentUpdaterConfiguration alloc] init];
MSGraphUpdateWindow *updateWindow = [[MSGraphUpdateWindow alloc] init];
[updateWindow setUpdateWindowStartTime:@"0:00:00"];
[updateWindow setUpdateWindowEndTime:@"23:59:00"];
[hybridAgentUpdaterConfiguration setUpdateWindow:updateWindow];

NSError *error;
NSData *hybridAgentUpdaterConfigurationData = [hybridAgentUpdaterConfiguration getSerializedDataWithError:&error];
[urlRequest setHTTPBody:hybridAgentUpdaterConfigurationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```