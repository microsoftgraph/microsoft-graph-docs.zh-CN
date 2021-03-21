---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a91ac78535c4c5a7ffd4501f47cc7dbfd7cb56ec
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963216"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphHybridAgentUpdaterConfiguration *hybridAgentUpdaterConfiguration = [[MSGraphHybridAgentUpdaterConfiguration alloc] init];
[hybridAgentUpdaterConfiguration setDeferUpdate:@"2018-08-20T12:00"];

NSError *error;
NSData *hybridAgentUpdaterConfigurationData = [hybridAgentUpdaterConfiguration getSerializedDataWithError:&error];
[urlRequest setHTTPBody:hybridAgentUpdaterConfigurationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```