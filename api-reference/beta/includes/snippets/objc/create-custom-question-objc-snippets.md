---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ddb81d20b8c579905487d86b7616ca4dbf37160
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105887"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/microsoft.graph.meetingRegistration/customQuestions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMeetingRegistrationQuestion *meetingRegistrationQuestion = [[MSGraphMeetingRegistrationQuestion alloc] init];
[meetingRegistrationQuestion setDisplayName:@"What's your job position?"];
[meetingRegistrationQuestion setIsRequired: false];
[meetingRegistrationQuestion setAnswerInputType: [MSGraphAnswerInputType text]];

NSError *error;
NSData *meetingRegistrationQuestionData = [meetingRegistrationQuestion getSerializedDataWithError:&error];
[urlRequest setHTTPBody:meetingRegistrationQuestionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```