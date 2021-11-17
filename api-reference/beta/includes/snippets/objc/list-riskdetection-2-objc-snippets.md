---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffd5490d4b62f1046c374e46a876988879ea8db18a6e32d08e61e4d0f761fc9d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220801"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityProtection/riskDetections/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphRiskDetection *riskDetection = [[MSGraphRiskDetection alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```