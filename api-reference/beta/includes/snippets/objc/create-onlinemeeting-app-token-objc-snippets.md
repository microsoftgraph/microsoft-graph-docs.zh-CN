---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 174582262af8bd5095beed4339638c6c36d4ca8b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995379"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/onlineMeetings"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOnlineMeeting *onlineMeeting = [[MSGraphOnlineMeeting alloc] init];
[onlineMeeting setIsBroadcast:@"false"];
[onlineMeeting setStartDateTime: "2019-09-09T21:33:30.8546353+00:00"];
[onlineMeeting setEndDateTime: "2019-09-09T22:03:30.8566356+00:00"];
[onlineMeeting setSubject:@"Application Token Meeting"];
MSGraphMeetingParticipants *participants = [[MSGraphMeetingParticipants alloc] init];
MSGraphMeetingParticipantInfo *organizer = [[MSGraphMeetingParticipantInfo alloc] init];
MSGraphIdentitySet *identity = [[MSGraphIdentitySet alloc] init];
MSGraphIdentity *user = [[MSGraphIdentity alloc] init];
[user setId:@"550fae72-d251-43ec-868c-373732c2704f"];
[identity setUser:user];
[organizer setIdentity:identity];
[participants setOrganizer:organizer];
[onlineMeeting setParticipants:participants];

NSError *error;
NSData *onlineMeetingData = [onlineMeeting getSerializedDataWithError:&error];
[urlRequest setHTTPBody:onlineMeetingData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```