---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e670602439ebcd8c4a989f49784e88ea2e2bd3fd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137656"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/dc17674c-81d9-4adb-bfb2-8f6a442e4622/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMeetingRegistrantBase *meetingRegistrantBase = [[MSGraphMeetingRegistrantBase alloc] init];
[meetingRegistrantBase setFirstName:@"Lisa"];
[meetingRegistrantBase setLastName:@"Adkins"];
[meetingRegistrantBase setEmail:@"lisa.adkins@contoso.com"];
NSMutableArray *customQuestionAnswersList = [[NSMutableArray alloc] init];
MSGraphCustomQuestionAnswer *customQuestionAnswers = [[MSGraphCustomQuestionAnswer alloc] init];
[customQuestionAnswers setQuestionId:@"MSM5YjlmM2Q4ZS03ZmVkLTRmN3gwMDIw94MDAyMF9hX3gwMDIwX2RldmU="];
[customQuestionAnswers setValue:@"No"];
[customQuestionAnswersList addObject: customQuestionAnswers];
MSGraphCustomQuestionAnswer *customQuestionAnswers = [[MSGraphCustomQuestionAnswer alloc] init];
[customQuestionAnswers setQuestionId:@"MSM5M2E2OWQ1Ni1jZTc4LTQDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8="];
[customQuestionAnswers setValue:@"Internet"];
[customQuestionAnswersList addObject: customQuestionAnswers];
[meetingRegistrantBase setCustomQuestionAnswers:customQuestionAnswersList];

NSError *error;
NSData *meetingRegistrantBaseData = [meetingRegistrantBase getSerializedDataWithError:&error];
[urlRequest setHTTPBody:meetingRegistrantBaseData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```