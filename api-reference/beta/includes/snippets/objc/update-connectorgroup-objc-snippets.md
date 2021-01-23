---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0d0ecabb4792ac2d2d059f3f2c3ed28cdbbf1e1
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945863"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/onPremisesPublishingProfiles/applicationProxy/connectorGroups"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphConnectorGroup *connectorGroup = [[MSGraphConnectorGroup alloc] init];
[connectorGroup setName:@"Connector Group Demo"];

NSError *error;
NSData *connectorGroupData = [connectorGroup getSerializedDataWithError:&error];
[urlRequest setHTTPBody:connectorGroupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```