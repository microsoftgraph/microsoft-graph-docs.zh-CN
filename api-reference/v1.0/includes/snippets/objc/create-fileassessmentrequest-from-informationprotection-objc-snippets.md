---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e14941c426185a41aeb716516c745e9ffc62c20
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42815869"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/informationProtection/threatAssessmentRequests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphThreatAssessmentRequest *threatAssessmentRequest = [[MSGraphThreatAssessmentRequest alloc] init];
[threatAssessmentRequest setExpectedAssessment: [MSGraphThreatExpectedAssessment block]];
[threatAssessmentRequest setCategory: [MSGraphThreatCategory malware]];
[threatAssessmentRequest setFileName:@"test.txt"];
[threatAssessmentRequest setContentData:@"VGhpcyBpcyBhIHRlc3QgZmlsZQ=="];

NSError *error;
NSData *threatAssessmentRequestData = [threatAssessmentRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:threatAssessmentRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```