---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cb5dada0c15fa86a4973bbdbf017fd96dddd404
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137659"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/16664f75-11dc-4870-bec6-38c1aaa81431/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMeetingRegistrantBase *meetingRegistrantBase = [[MSGraphMeetingRegistrantBase alloc] init];
[meetingRegistrantBase setFirstName:@"Frederick"];
[meetingRegistrantBase setLastName:@"Cormier"];
[meetingRegistrantBase setEmail:@"frederick.cormier@contoso.com"];
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