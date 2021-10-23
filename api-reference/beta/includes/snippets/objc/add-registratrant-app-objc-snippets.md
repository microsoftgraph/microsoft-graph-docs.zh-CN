---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbe60f24b7ba0f9946790fc6e8aea6bb7c165257
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561694"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/dc17674c-81d9-4adb-bfb2-8f6a442e4622/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMeetingRegistrant *meetingRegistrant = [[MSGraphMeetingRegistrant alloc] init];
[meetingRegistrant setFirstName:@"Lisa"];
[meetingRegistrant setLastName:@"Adkins"];
[meetingRegistrant setEmail:@"lisa.adkins@contoso.com"];
NSMutableArray *customQuestionAnswersList = [[NSMutableArray alloc] init];
MSGraphCustomQuestionAnswer *customQuestionAnswers = [[MSGraphCustomQuestionAnswer alloc] init];
[customQuestionAnswers setQuestionId:@"MSM5YjlmM2Q4ZS03ZmVkLTRmN3gwMDIw94MDAyMF9hX3gwMDIwX2RldmU="];
[customQuestionAnswers setValue:@"No"];
[customQuestionAnswersList addObject: customQuestionAnswers];
MSGraphCustomQuestionAnswer *customQuestionAnswers = [[MSGraphCustomQuestionAnswer alloc] init];
[customQuestionAnswers setQuestionId:@"MSM5M2E2OWQ1Ni1jZTc4LTQDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8="];
[customQuestionAnswers setValue:@"Internet"];
[customQuestionAnswersList addObject: customQuestionAnswers];
[meetingRegistrant setCustomQuestionAnswers:customQuestionAnswersList];

NSError *error;
NSData *meetingRegistrantData = [meetingRegistrant getSerializedDataWithError:&error];
[urlRequest setHTTPBody:meetingRegistrantData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```