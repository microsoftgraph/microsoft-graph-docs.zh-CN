---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a076fb57160c3ea33ac2cf52d7d78e1dbecf96c100ec943b6b592f011d432b75
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161465"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/informationProtection/threatAssessmentRequests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphThreatAssessmentRequest *threatAssessmentRequest = [[MSGraphThreatAssessmentRequest alloc] init];
[threatAssessmentRequest setRecipientEmail:@"tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com"];
[threatAssessmentRequest setExpectedAssessment: [MSGraphThreatExpectedAssessment block]];
[threatAssessmentRequest setCategory: [MSGraphThreatCategory malware]];
[threatAssessmentRequest setContentData:@"UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC....."];

NSError *error;
NSData *threatAssessmentRequestData = [threatAssessmentRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:threatAssessmentRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```