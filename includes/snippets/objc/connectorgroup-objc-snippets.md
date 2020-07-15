---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0d30c7b3274bb2735227c92e34d71ae10f9395f
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142353"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83/connectorGroup/$ref"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphConnectorGroup *connectorGroup = [[MSGraphConnectorGroup alloc] init];

NSError *error;
NSData *connectorGroupData = [connectorGroup getSerializedDataWithError:&error];
[urlRequest setHTTPBody:connectorGroupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```