---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee70b15106d9f2e28b0b28213e2b3a88758faca8
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "40867144"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/informationProtection/threatAssessmentRequests/ab2ad9b3-2213-4091-ae0c-08d76ddbcacf"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphThreatAssessmentRequest *threatAssessmentRequest = [[MSGraphThreatAssessmentRequest alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```