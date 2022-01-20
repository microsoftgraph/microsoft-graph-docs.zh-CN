---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32f5c026346b44a32c25e95a2ee729b079cb78f4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106894"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customQuestions/3bc6fde0-4ad3-445d-ab17-0fc15dba0774"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphBookingCustomQuestion *bookingCustomQuestion = [[MSGraphBookingCustomQuestion alloc] init];
[bookingCustomQuestion setDisplayName:@"What is your age?"];
[bookingCustomQuestion setAnswerInputType: [MSGraphAnswerInputType text]];
NSMutableArray *answerOptionsList = [[NSMutableArray alloc] init];
[bookingCustomQuestion setAnswerOptions:answerOptionsList];

NSError *error;
NSData *bookingCustomQuestionData = [bookingCustomQuestion getSerializedDataWithError:&error];
[urlRequest setHTTPBody:bookingCustomQuestionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```