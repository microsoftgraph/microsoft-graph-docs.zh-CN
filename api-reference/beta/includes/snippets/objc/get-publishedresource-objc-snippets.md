---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 275c4f204cf347e9585884abe65f908ce56c80d092041fd71b991d5a1f8d5632
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163086"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/onPremisesPublishingProfiles/provisioning/publishedResources/aed0b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphPublishedResource *publishedResource = [[MSGraphPublishedResource alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```