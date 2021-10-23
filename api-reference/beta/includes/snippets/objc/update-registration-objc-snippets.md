---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c01dc7cc1a2b4d0c778d0fc7fb3694b57314ce1
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561021"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMeetingRegistration *meetingRegistration = [[MSGraphMeetingRegistration alloc] init];
[meetingRegistration setSubject:@"Microsoft Ignite: Day 1"];
[meetingRegistration setStartDateTime: "2021-11-02T16:00:00+00:00"];
[meetingRegistration setEndDateTime: "2021-11-02T23:45:00+00:00"];
NSMutableArray *speakersList = [[NSMutableArray alloc] init];
MSGraphMeetingSpeaker *speakers = [[MSGraphMeetingSpeaker alloc] init];
[speakers setDisplayName:@"Henry Ross"];
[speakers setBio:@"Chairman and Chief Executive Officer"];
[speakersList addObject: speakers];
MSGraphMeetingSpeaker *speakers = [[MSGraphMeetingSpeaker alloc] init];
[speakers setDisplayName:@"Fred Ryan"];
[speakers setBio:@"CVP"];
[speakersList addObject: speakers];
[meetingRegistration setSpeakers:speakersList];

NSError *error;
NSData *meetingRegistrationData = [meetingRegistration getSerializedDataWithError:&error];
[urlRequest setHTTPBody:meetingRegistrationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```