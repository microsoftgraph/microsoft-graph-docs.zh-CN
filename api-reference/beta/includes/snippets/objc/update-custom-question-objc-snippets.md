---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83de7a1ff6c98bbfd3c899c97f10595fcfbdc133
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60558613"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/customQuestions/MSNhYjc5NWI4MC119zX3gwMDIwX3lvdXJfeDAwMjBfam8="]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMeetingRegistrationQuestion *meetingRegistrationQuestion = [[MSGraphMeetingRegistrationQuestion alloc] init];
[meetingRegistrationQuestion setAnswerInputType: [MSGraphAnswerInputType radioButton]];
NSMutableArray *answerOptionsList = [[NSMutableArray alloc] init];
[answerOptionsList addObject: @"Software Engineer"];
[answerOptionsList addObject: @"Software Development Manager"];
[answerOptionsList addObject: @"Product Manager"];
[answerOptionsList addObject: @"Data scientist"];
[answerOptionsList addObject: @"Other"];
[meetingRegistrationQuestion setAnswerOptions:answerOptionsList];

NSError *error;
NSData *meetingRegistrationQuestionData = [meetingRegistrationQuestion getSerializedDataWithError:&error];
[urlRequest setHTTPBody:meetingRegistrationQuestionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```