---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a7a85616954d8d6e7c64ad0ca3d5fe9c6f2d015
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "41494584"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/riskDetections"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphRiskDetection *riskDetection = [[MSGraphRiskDetection alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```